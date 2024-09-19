# BigQueryの使い方

```text
データセット ID
bigquery-public-data.ga4_obfuscated_sample_ecommerce

作成
2021/08/11, 7:27:49 UTC+9

デフォルトのテーブルの有効期限
なし

最終更新
2022/09/20, 16:43:30 UTC+9

データのロケーション
US

説明
Obfuscated Google Analytics 4 data emulating a web ecommerce implementation of Google Analytics. It’s a great way to look at business data and experiment and learn the benefits of analyzing Google Analytics data in BigQuery. Learn more at: https://developers.google.com/analytics/bigquery/web-ecommerce-demo-dataset

デフォルトの照合

デフォルトの丸めモード
ROUNDING_MODE_UNSPECIFIED

大文字 / 小文字の区別なし
false

ラベル

```

```sql
select
  distinct event_date
from
  `bigquery-public-data.ga4_obfuscated_sample_ecommerce.events_2021013*`
```


```sql
-- 作成先のDBとテーブル名を記載
create or replace table `[サーバー名].sandbox.access_log_ga4` as

-- 実行内容 
with session_id_tb as (
  select
    event_date,
    event_name,
    user_pseudo_id,
    (SELECT value.int_value FROM UNNEST(event_params) WHERE key = 'ga_session_id') AS ga_session_id,
  from
    `bigquery-public-data.ga4_obfuscated_sample_ecommerce.events_202101*`
)
select
  user_pseudo_id,
  count(distinct concat(user_pseudo_id, ga_session_id)) as session_num,
  countif(event_name = 'page_view') as pv_num,
  countif(event_name = 'purchase') as purchase_num
from
  session_id_tb
group by user_pseudo_id
order by session_num desc, pv_num desc
```

