# Chinese Simplified (zh-CN) locale

## `format` and `parse`

| Title                           | Token string | Date                     | `format` result                                   | `parse` result           |
| ------------------------------- | ------------ | ------------------------ | ------------------------------------------------- | ------------------------ |
| Calendar year                   | yo           | 1987-02-11T12:13:14.015Z | 第 1987                                           | 1987-01-01T00:00:00.000Z |
|                                 |              | 0005-01-01T12:13:14.015Z | 第 5                                              | 0005-01-01T00:00:00.000Z |
| Local week-numbering year       | Yo           | 1987-02-11T12:13:14.015Z | 第 1987                                           | 1986-12-29T00:00:00.000Z |
|                                 |              | 0005-01-01T12:13:14.015Z | 第 4                                              | 0003-12-29T00:00:00.000Z |
| Quarter (formatting)            | Qo           | 2019-01-01T12:13:14.015Z | 第 1                                              | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 第 2                                              | 2019-04-01T00:00:00.000Z |
|                                 | QQQ          | 2019-01-01T12:13:14.015Z | 第一季                                            | Invalid Date             |
|                                 |              | 2019-04-01T12:13:14.015Z | 第二季                                            | Invalid Date             |
|                                 | QQQQ         | 2019-01-01T12:13:14.015Z | 第一季度                                          | Invalid Date             |
|                                 |              | 2019-04-01T12:13:14.015Z | 第二季度                                          | Invalid Date             |
|                                 | QQQQQ        | 2019-01-01T12:13:14.015Z | 1                                                 | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 2                                                 | 2019-04-01T00:00:00.000Z |
| Quarter (stand-alone)           | qo           | 2019-01-01T12:13:14.015Z | 第 1                                              | 2019-01-01T00:00:00.000Z |
|                                 |              | 2019-04-01T12:13:14.015Z | 第 2                                              | 2019-04-01T00:00:00.000Z |
|                                 | qqq          | 2019-01-01T12:13:14.015Z | 第一季                                            | Invalid Date             |
|                                 |              | 2019-04-01T12:13:14.015Z | 第二季                                            | Invalid Date             |
|                                 | qqqq         | 2019-01-01T12:13:14.015Z | 第一季度                                          | Invalid Date             |
|                                 |              | 2019-04-01T12:13:14.015Z | 第二季度                                          | Invalid Date             |
| Month (formatting)              | Mo           | 2019-02-11T12:13:14.015Z | 第 2                                              | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 第 7                                              | 2019-07-01T00:00:00.000Z |
|                                 | MMM          | 2019-02-11T12:13:14.015Z | 2 月                                              | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 7 月                                              | 2019-07-01T00:00:00.000Z |
|                                 | MMMM         | 2019-02-11T12:13:14.015Z | 二月                                              | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 七月                                              | 2019-07-01T00:00:00.000Z |
|                                 | MMMMM        | 2019-02-11T12:13:14.015Z | 二                                                | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 七                                                | 2019-07-01T00:00:00.000Z |
| Month (stand-alone)             | Lo           | 2019-02-11T12:13:14.015Z | 第 2                                              | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 第 7                                              | 2019-07-01T00:00:00.000Z |
|                                 | LLL          | 2019-02-11T12:13:14.015Z | 2 月                                              | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 7 月                                              | 2019-07-01T00:00:00.000Z |
|                                 | LLLL         | 2019-02-11T12:13:14.015Z | 二月                                              | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 七月                                              | 2019-07-01T00:00:00.000Z |
|                                 | LLLLL        | 2019-02-11T12:13:14.015Z | 二                                                | 2019-02-01T00:00:00.000Z |
|                                 |              | 2019-07-10T12:13:14.015Z | 七                                                | 2019-07-01T00:00:00.000Z |
| Local week of year              | wo           | 2019-01-01T12:13:14.015Z | 第 1                                              | 2018-12-31T00:00:00.000Z |
|                                 |              | 2019-12-01T12:13:14.015Z | 第 48                                             | 2019-11-25T00:00:00.000Z |
| ISO week of year                | Io           | 2019-01-01T12:13:14.015Z | 第 1                                              | 2018-12-31T00:00:00.000Z |
|                                 |              | 2019-12-01T12:13:14.015Z | 第 48                                             | 2019-11-25T00:00:00.000Z |
| Day of month                    | do           | 2019-02-11T12:13:14.015Z | 11 日                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-28T12:13:14.015Z | 28 日                                             | 2019-02-28T00:00:00.000Z |
| Day of year                     | Do           | 2019-02-11T12:13:14.015Z | 第 42                                             | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-12-31T12:13:14.015Z | 第 365                                            | 2019-12-31T00:00:00.000Z |
| Day of week (formatting)        | E            | 2019-02-11T12:13:14.015Z | 周一                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 周五                                              | 2019-02-15T00:00:00.000Z |
|                                 | EE           | 2019-02-11T12:13:14.015Z | 周一                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 周五                                              | 2019-02-15T00:00:00.000Z |
|                                 | EEE          | 2019-02-11T12:13:14.015Z | 周一                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 周五                                              | 2019-02-15T00:00:00.000Z |
|                                 | EEEE         | 2019-02-11T12:13:14.015Z | 星期一                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 星期五                                            | 2019-02-15T00:00:00.000Z |
|                                 | EEEEE        | 2019-02-11T12:13:14.015Z | 一                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 五                                                | 2019-02-15T00:00:00.000Z |
|                                 | EEEEEE       | 2019-02-11T12:13:14.015Z | 一                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 五                                                | 2019-02-15T00:00:00.000Z |
| ISO day of week (formatting)    | io           | 2019-02-11T12:13:14.015Z | 第 1                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 第 5                                              | 2019-02-15T00:00:00.000Z |
|                                 | iii          | 2019-02-11T12:13:14.015Z | 周一                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 周五                                              | 2019-02-15T00:00:00.000Z |
|                                 | iiii         | 2019-02-11T12:13:14.015Z | 星期一                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 星期五                                            | 2019-02-15T00:00:00.000Z |
|                                 | iiiii        | 2019-02-11T12:13:14.015Z | 一                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 五                                                | 2019-02-15T00:00:00.000Z |
|                                 | iiiiii       | 2019-02-11T12:13:14.015Z | 一                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 五                                                | 2019-02-15T00:00:00.000Z |
| Local day of week (formatting)  | eo           | 2019-02-11T12:13:14.015Z | 第 1                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 第 5                                              | 2019-02-15T00:00:00.000Z |
|                                 | eee          | 2019-02-11T12:13:14.015Z | 周一                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 周五                                              | 2019-02-15T00:00:00.000Z |
|                                 | eeee         | 2019-02-11T12:13:14.015Z | 星期一                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 星期五                                            | 2019-02-15T00:00:00.000Z |
|                                 | eeeee        | 2019-02-11T12:13:14.015Z | 一                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 五                                                | 2019-02-15T00:00:00.000Z |
|                                 | eeeeee       | 2019-02-11T12:13:14.015Z | 一                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 五                                                | 2019-02-15T00:00:00.000Z |
| Local day of week (stand-alone) | co           | 2019-02-11T12:13:14.015Z | 第 1                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 第 5                                              | 2019-02-15T00:00:00.000Z |
|                                 | ccc          | 2019-02-11T12:13:14.015Z | 周一                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 周五                                              | 2019-02-15T00:00:00.000Z |
|                                 | cccc         | 2019-02-11T12:13:14.015Z | 星期一                                            | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 星期五                                            | 2019-02-15T00:00:00.000Z |
|                                 | ccccc        | 2019-02-11T12:13:14.015Z | 一                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 五                                                | 2019-02-15T00:00:00.000Z |
|                                 | cccccc       | 2019-02-11T12:13:14.015Z | 一                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-15T12:13:14.015Z | 五                                                | 2019-02-15T00:00:00.000Z |
| AM, PM                          | a            | 2019-02-11T11:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 | aa           | 2019-02-11T11:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 | aaa          | 2019-02-11T11:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 | aaaa         | 2019-02-11T11:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 | aaaaa        | 2019-02-11T11:13:14.015Z | 上                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下                                                | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 下                                                | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 上                                                | 2019-02-11T00:00:00.000Z |
| AM, PM, noon, midnight          | b            | 2019-02-11T11:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 | bb           | 2019-02-11T11:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 | bbb          | 2019-02-11T11:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 | bbbb         | 2019-02-11T11:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 上午                                              | 2019-02-11T00:00:00.000Z |
|                                 | bbbbb        | 2019-02-11T11:13:14.015Z | 上                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下                                                | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 下                                                | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 上                                                | 2019-02-11T00:00:00.000Z |
| Flexible day period             | B            | 2019-02-11T11:13:14.015Z | 早晨                                              | Invalid Date             |
|                                 |              | 2019-02-11T14:13:14.015Z | 中午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 晚上                                              | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 夜间                                              | Invalid Date             |
|                                 | BB           | 2019-02-11T11:13:14.015Z | 早晨                                              | Invalid Date             |
|                                 |              | 2019-02-11T14:13:14.015Z | 中午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 晚上                                              | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 夜间                                              | Invalid Date             |
|                                 | BBB          | 2019-02-11T11:13:14.015Z | 早晨                                              | Invalid Date             |
|                                 |              | 2019-02-11T14:13:14.015Z | 中午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 晚上                                              | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 夜间                                              | Invalid Date             |
|                                 | BBBB         | 2019-02-11T11:13:14.015Z | 早晨                                              | Invalid Date             |
|                                 |              | 2019-02-11T14:13:14.015Z | 中午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 晚上                                              | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 夜间                                              | Invalid Date             |
|                                 | BBBBB        | 2019-02-11T11:13:14.015Z | 早                                                | 2019-02-11T00:00:00.000Z |
|                                 |              | 2019-02-11T14:13:14.015Z | 下午                                              | 2019-02-11T12:00:00.000Z |
|                                 |              | 2019-02-11T19:13:14.015Z | 晚                                                | 2019-02-11T17:00:00.000Z |
|                                 |              | 2019-02-11T02:13:14.015Z | 夜                                                | Invalid Date             |
| Hour [1-12]                     | ho           | 2019-02-11T11:13:14.015Z | 11 时                                             | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 11 时                                             | 2019-02-11T23:00:00.000Z |
| Hour [0-23]                     | Ho           | 2019-02-11T11:13:14.015Z | 11 时                                             | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 23 时                                             | 2019-02-11T23:00:00.000Z |
| Hour [0-11]                     | Ko           | 2019-02-11T11:13:14.015Z | 11 时                                             | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 11 时                                             | 2019-02-11T23:00:00.000Z |
| Hour [1-24]                     | ko           | 2019-02-11T11:13:14.015Z | 11 时                                             | 2019-02-11T11:00:00.000Z |
|                                 |              | 2019-02-11T23:13:14.015Z | 23 时                                             | 2019-02-11T23:00:00.000Z |
| Minute                          | mo           | 2019-01-01T12:01:14.015Z | 1 分                                              | 2019-01-01T12:01:00.000Z |
|                                 |              | 2019-04-01T12:55:14.015Z | 55 分                                             | 2019-04-01T12:55:00.000Z |
| Second                          | so           | 2019-01-01T12:13:01.015Z | 1 秒                                              | 2019-01-01T12:13:01.000Z |
|                                 |              | 2019-04-01T12:13:55.015Z | 55 秒                                             | 2019-04-01T12:13:55.000Z |
| Long localized date             | P            | 1987-02-11T12:13:14.015Z | 87-02-11                                          | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 53-05-29                                          | 1453-05-29T00:00:00.000Z |
|                                 | PP           | 1987-02-11T12:13:14.015Z | 1987-02-11                                        | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 1453-05-29                                        | 1453-05-29T00:00:00.000Z |
|                                 | PPP          | 1987-02-11T12:13:14.015Z | 1987 年 2 月 11 日                                | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 1453 年 5 月 29 日                                | 1453-05-29T00:00:00.000Z |
|                                 | PPPP         | 1987-02-11T12:13:14.015Z | 1987 年 2 月 11 日 星期三                         | 1987-02-11T00:00:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 1453 年 5 月 29 日 星期日                         | 1453-05-29T00:00:00.000Z |
| Long localized time             | p            | 1987-02-11T12:13:14.015Z | 下午 12:13                                        | 1987-02-11T12:13:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 下午 11:59                                        | 1453-05-29T23:59:00.000Z |
|                                 | pp           | 1987-02-11T12:13:14.015Z | 下午 12:13:14                                     | 1987-02-11T12:13:14.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 下午 11:59:59                                     | 1453-05-29T23:59:59.000Z |
|                                 | ppp          | 1987-02-11T12:13:14.015Z | GMT+0 下午 12:13:14                               | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | GMT+0 下午 11:59:59                               | Errored                  |
|                                 | pppp         | 1987-02-11T12:13:14.015Z | GMT+00:00 下午 12:13:14                           | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | GMT+00:00 下午 11:59:59                           | Errored                  |
| Combination of date and time    | Pp           | 1987-02-11T12:13:14.015Z | 87-02-11 下午 12:13                               | 1987-02-11T12:13:00.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 53-05-29 下午 11:59                               | 1453-05-29T23:59:00.000Z |
|                                 | PPpp         | 1987-02-11T12:13:14.015Z | 1987-02-11 下午 12:13:14                          | 1987-02-11T12:13:14.000Z |
|                                 |              | 1453-05-29T23:59:59.999Z | 1453-05-29 下午 11:59:59                          | 1453-05-29T23:59:59.000Z |
|                                 | PPPppp       | 1987-02-11T12:13:14.015Z | 1987 年 2 月 11 日 GMT+0 下午 12:13:14            | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 1453 年 5 月 29 日 GMT+0 下午 11:59:59            | Errored                  |
|                                 | PPPPpppp     | 1987-02-11T12:13:14.015Z | 1987 年 2 月 11 日 星期三 GMT+00:00 下午 12:13:14 | Errored                  |
|                                 |              | 1453-05-29T23:59:59.999Z | 1453 年 5 月 29 日 星期日 GMT+00:00 下午 11:59:59 | Errored                  |

## `formatDistance`

If now is January 1st, 2000, 00:00.

| Date                     | Result      | `includeSeconds: true` | `addSuffix: true` |
| ------------------------ | ----------- | ---------------------- | ----------------- |
| 2006-01-01T00:00:00.000Z | 大约 6 年   | 大约 6 年              | 大约 6 年内       |
| 2005-01-01T00:00:00.000Z | 大约 5 年   | 大约 5 年              | 大约 5 年内       |
| 2004-01-01T00:00:00.000Z | 大约 4 年   | 大约 4 年              | 大约 4 年内       |
| 2003-01-01T00:00:00.000Z | 大约 3 年   | 大约 3 年              | 大约 3 年内       |
| 2002-01-01T00:00:00.000Z | 大约 2 年   | 大约 2 年              | 大约 2 年内       |
| 2001-06-01T00:00:00.000Z | 超过 1 年   | 超过 1 年              | 超过 1 年内       |
| 2001-02-01T00:00:00.000Z | 大约 1 年   | 大约 1 年              | 大约 1 年内       |
| 2001-01-01T00:00:00.000Z | 大约 1 年   | 大约 1 年              | 大约 1 年内       |
| 2000-06-01T00:00:00.000Z | 5 个月      | 5 个月                 | 5 个月内          |
| 2000-03-01T00:00:00.000Z | 2 个月      | 2 个月                 | 2 个月内          |
| 2000-02-01T00:00:00.000Z | 大约 1 个月 | 大约 1 个月            | 大约 1 个月内     |
| 2000-01-15T00:00:00.000Z | 14 天       | 14 天                  | 14 天内           |
| 2000-01-02T00:00:00.000Z | 1 天        | 1 天                   | 1 天内            |
| 2000-01-01T06:00:00.000Z | 大约 6 小时 | 大约 6 小时            | 大约 6 小时内     |
| 2000-01-01T01:00:00.000Z | 大约 1 小时 | 大约 1 小时            | 大约 1 小时内     |
| 2000-01-01T00:45:00.000Z | 大约 1 小时 | 大约 1 小时            | 大约 1 小时内     |
| 2000-01-01T00:30:00.000Z | 30 分钟     | 30 分钟                | 30 分钟内         |
| 2000-01-01T00:15:00.000Z | 15 分钟     | 15 分钟                | 15 分钟内         |
| 2000-01-01T00:01:00.000Z | 1 分钟      | 1 分钟                 | 1 分钟内          |
| 2000-01-01T00:00:25.000Z | 不到 1 分钟 | 半分钟                 | 不到 1 分钟内     |
| 2000-01-01T00:00:15.000Z | 不到 1 分钟 | 不到 20 秒             | 不到 1 分钟内     |
| 2000-01-01T00:00:05.000Z | 不到 1 分钟 | 不到 10 秒             | 不到 1 分钟内     |
| 2000-01-01T00:00:00.000Z | 不到 1 分钟 | 不到 5 秒              | 不到 1 分钟前     |
| 1999-12-31T23:59:55.000Z | 不到 1 分钟 | 不到 10 秒             | 不到 1 分钟前     |
| 1999-12-31T23:59:45.000Z | 不到 1 分钟 | 不到 20 秒             | 不到 1 分钟前     |
| 1999-12-31T23:59:35.000Z | 不到 1 分钟 | 半分钟                 | 不到 1 分钟前     |
| 1999-12-31T23:59:00.000Z | 1 分钟      | 1 分钟                 | 1 分钟前          |
| 1999-12-31T23:45:00.000Z | 15 分钟     | 15 分钟                | 15 分钟前         |
| 1999-12-31T23:30:00.000Z | 30 分钟     | 30 分钟                | 30 分钟前         |
| 1999-12-31T23:15:00.000Z | 大约 1 小时 | 大约 1 小时            | 大约 1 小时前     |
| 1999-12-31T23:00:00.000Z | 大约 1 小时 | 大约 1 小时            | 大约 1 小时前     |
| 1999-12-31T18:00:00.000Z | 大约 6 小时 | 大约 6 小时            | 大约 6 小时前     |
| 1999-12-30T00:00:00.000Z | 2 天        | 2 天                   | 2 天前            |
| 1999-12-15T00:00:00.000Z | 17 天       | 17 天                  | 17 天前           |
| 1999-12-01T00:00:00.000Z | 大约 1 个月 | 大约 1 个月            | 大约 1 个月前     |
| 1999-11-01T00:00:00.000Z | 2 个月      | 2 个月                 | 2 个月前          |
| 1999-06-01T00:00:00.000Z | 7 个月      | 7 个月                 | 7 个月前          |
| 1999-01-01T00:00:00.000Z | 大约 1 年   | 大约 1 年              | 大约 1 年前       |
| 1998-12-01T00:00:00.000Z | 大约 1 年   | 大约 1 年              | 大约 1 年前       |
| 1998-06-01T00:00:00.000Z | 超过 1 年   | 超过 1 年              | 超过 1 年前       |
| 1998-01-01T00:00:00.000Z | 大约 2 年   | 大约 2 年              | 大约 2 年前       |
| 1997-01-01T00:00:00.000Z | 大约 3 年   | 大约 3 年              | 大约 3 年前       |
| 1996-01-01T00:00:00.000Z | 大约 4 年   | 大约 4 年              | 大约 4 年前       |
| 1995-01-01T00:00:00.000Z | 大约 5 年   | 大约 5 年              | 大约 5 年前       |
| 1994-01-01T00:00:00.000Z | 大约 6 年   | 大约 6 年              | 大约 6 年前       |

## `formatDistanceStrict`

If now is January 1st, 2000, 00:00.

| Date                     | Result  | `addSuffix: true` | With forced unit (i.e. `hour`) |
| ------------------------ | ------- | ----------------- | ------------------------------ |
| 2006-01-01T00:00:00.000Z | 6 年    | 6 年内            | 52608 小时                     |
| 2005-01-01T00:00:00.000Z | 5 年    | 5 年内            | 43848 小时                     |
| 2004-01-01T00:00:00.000Z | 4 年    | 4 年内            | 35064 小时                     |
| 2003-01-01T00:00:00.000Z | 3 年    | 3 年内            | 26304 小时                     |
| 2002-01-01T00:00:00.000Z | 2 年    | 2 年内            | 17544 小时                     |
| 2001-06-01T00:00:00.000Z | 1 年    | 1 年内            | 12408 小时                     |
| 2001-02-01T00:00:00.000Z | 1 年    | 1 年内            | 9528 小时                      |
| 2001-01-01T00:00:00.000Z | 1 年    | 1 年内            | 8784 小时                      |
| 2000-06-01T00:00:00.000Z | 5 个月  | 5 个月内          | 3648 小时                      |
| 2000-03-01T00:00:00.000Z | 2 个月  | 2 个月内          | 1440 小时                      |
| 2000-02-01T00:00:00.000Z | 1 个月  | 1 个月内          | 744 小时                       |
| 2000-01-15T00:00:00.000Z | 14 天   | 14 天内           | 336 小时                       |
| 2000-01-02T00:00:00.000Z | 1 天    | 1 天内            | 24 小时                        |
| 2000-01-01T06:00:00.000Z | 6 小时  | 6 小时内          | 6 小时                         |
| 2000-01-01T01:00:00.000Z | 1 小时  | 1 小时内          | 1 小时                         |
| 2000-01-01T00:45:00.000Z | 45 分钟 | 45 分钟内         | 1 小时                         |
| 2000-01-01T00:30:00.000Z | 30 分钟 | 30 分钟内         | 1 小时                         |
| 2000-01-01T00:15:00.000Z | 15 分钟 | 15 分钟内         | 0 小时                         |
| 2000-01-01T00:01:00.000Z | 1 分钟  | 1 分钟内          | 0 小时                         |
| 2000-01-01T00:00:25.000Z | 25 秒   | 25 秒内           | 0 小时                         |
| 2000-01-01T00:00:15.000Z | 15 秒   | 15 秒内           | 0 小时                         |
| 2000-01-01T00:00:05.000Z | 5 秒    | 5 秒内            | 0 小时                         |
| 2000-01-01T00:00:00.000Z | 0 秒    | 0 秒前            | 0 小时                         |
| 1999-12-31T23:59:55.000Z | 5 秒    | 5 秒前            | 0 小时                         |
| 1999-12-31T23:59:45.000Z | 15 秒   | 15 秒前           | 0 小时                         |
| 1999-12-31T23:59:35.000Z | 25 秒   | 25 秒前           | 0 小时                         |
| 1999-12-31T23:59:00.000Z | 1 分钟  | 1 分钟前          | 0 小时                         |
| 1999-12-31T23:45:00.000Z | 15 分钟 | 15 分钟前         | 0 小时                         |
| 1999-12-31T23:30:00.000Z | 30 分钟 | 30 分钟前         | 1 小时                         |
| 1999-12-31T23:15:00.000Z | 45 分钟 | 45 分钟前         | 1 小时                         |
| 1999-12-31T23:00:00.000Z | 1 小时  | 1 小时前          | 1 小时                         |
| 1999-12-31T18:00:00.000Z | 6 小时  | 6 小时前          | 6 小时                         |
| 1999-12-30T00:00:00.000Z | 2 天    | 2 天前            | 48 小时                        |
| 1999-12-15T00:00:00.000Z | 17 天   | 17 天前           | 408 小时                       |
| 1999-12-01T00:00:00.000Z | 1 个月  | 1 个月前          | 744 小时                       |
| 1999-11-01T00:00:00.000Z | 2 个月  | 2 个月前          | 1464 小时                      |
| 1999-06-01T00:00:00.000Z | 7 个月  | 7 个月前          | 5136 小时                      |
| 1999-01-01T00:00:00.000Z | 1 年    | 1 年前            | 8760 小时                      |
| 1998-12-01T00:00:00.000Z | 1 年    | 1 年前            | 9504 小时                      |
| 1998-06-01T00:00:00.000Z | 2 年    | 2 年前            | 13896 小时                     |
| 1998-01-01T00:00:00.000Z | 2 年    | 2 年前            | 17520 小时                     |
| 1997-01-01T00:00:00.000Z | 3 年    | 3 年前            | 26280 小时                     |
| 1996-01-01T00:00:00.000Z | 4 年    | 4 年前            | 35064 小时                     |
| 1995-01-01T00:00:00.000Z | 5 年    | 5 年前            | 43824 小时                     |
| 1994-01-01T00:00:00.000Z | 6 年    | 6 年前            | 52584 小时                     |

## `formatRelative`

If now is January 1st, 2000, 00:00.

| Date                     | Result                |
| ------------------------ | --------------------- |
| 2000-01-10T00:00:00.000Z | 2000-01-10 上午 12:00 |
| 2000-01-05T00:00:00.000Z | 下个星期三 上午 12:00 |
| 2000-01-02T00:00:00.000Z | 明天 上午 12:00       |
| 2000-01-01T00:00:00.000Z | 今天 上午 12:00       |
| 1999-12-31T00:00:00.000Z | 昨天 上午 12:00       |
| 1999-12-27T00:00:00.000Z | 星期一 上午 12:00     |
| 1999-12-21T00:00:00.000Z | 1999-12-21 上午 12:00 |
