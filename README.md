# 小工具---自动生成虚拟币收益数据
## 下载
- [windows](https://github.com/K1ngram4/CoinRecord/releases/download/V1.0/CoinRecord_windows.zip)
- [osx](https://github.com/K1ngram4/CoinRecord/releases/download/V1.0/CoinRecord_mac.zip)

执行可执行文件即可在records目录下生成md文件，记录收益数据

- 效果

| 币种 | 持有数量       | 现价         | 总金额      | 持仓均价     | 成本        | 利润      | 收益率 |
| ---- | -------------- | ------------ | ----------- | ------------ | ----------- | --------- | ------ |
| btc  | 0.013343       | 45168.320300 | 602.680898  | 41737.240501 | 556.900000  | 45.780898 | 8.22%  |
| doge | 8058.726300    | 0.299873     | 2416.596306 | 0.297150     | 2394.650000 | 21.946306 | 0.92%  |
| icp  | 0.718261       | 57.868641    | 41.564765   | 57.138036    | 41.040000   | 0.524765  | 1.28%  |
| shib | 3460860.410000 | 0.000008     | 28.326569   | 0.000008     | 28.240000   | 0.086569  | 0.31%  |
| win  | 9991.000000    | 0.000635     | 6.340803    | 0.000621     | 6.200000    | 0.140803  | 2.27%  |


## 配置说明
- 配置文件在holds目录下，json格式，多条记录分开
```json
{
  "name": "btc",
  "records": [
    {
     "operate": "+",
     "amount": 0.01329424,
     "sum": 613.82
    },
    {
     "operate": "-",
     "amount": 0.01329424,
     "sum": 613.82
    }
  ]
}
```
- name 币种
- records 表示操作记录
  - opetare 操作 “+”买入   “-”卖出
  - amount 数量
  - sum 总金额 单位usdt

**一个币种一个json文件**