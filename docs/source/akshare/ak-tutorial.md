# 10分钟快速入门

## 1. 先进行 [AkShare](https://github.com/jindaxiang/akshare) 环境配置

## 2. 再查看 [AkShare](https://github.com/jindaxiang/akshare) 提供的数据接口

具体函数使用详情, 请查看 [AkShare 文档](https://akshare.readthedocs.io/) 每个接口的示例代码

[AkShare](https://github.com/jindaxiang/akshare) 数据接口一览表

```
 # 交易所期货数据
 "get_cffex_daily",  # 获取中国金融期货交易所每日交易数据
 "get_cffex_rank_table",  # 获取中国金融期货交易所前20会员持仓数据明细
 "get_czce_daily",  # 获取郑州商品交易所每日交易数据
 "get_czce_rank_table",  # 获取郑州商品交易所前20会员持仓数据明细
 "get_dce_daily",  # 获取大连商品交易所每日交易数据
 "get_dce_rank_table",  #获取大连商品交易所前20会员持仓数据明细
 "get_futures_daily",  # 获取中国金融期货交易所每日基差数据
 "get_rank_sum",  # 获取四个期货交易所前5, 10, 15, 20会员持仓排名数据
 "get_rank_sum_daily",  # 获取每日四个期货交易所前5, 10, 15, 20会员持仓排名数据
 "get_receipt",  # 获取大宗商品注册仓单数据
 "get_roll_yield",  # 获取某一天某品种(主力和次主力)或固定两个合约的展期收益率
 "get_roll_yield_bar",  # 获取展期收益率
 "get_shfe_daily",  # 获取上海期货交易所每日交易数据
 "get_shfe_rank_table",  # 获取上海期货交易所前20会员持仓数据明细
 "get_shfe_v_wap",  # 获取上海期货交易所日成交均价数据
 "get_spot_price",  # 获取某一交易日大宗商品现货价格及相应基差数据
 "get_spot_price_daily"  # 获取一段交易日大宗商品现货价格及相应基差数据
 # 奇货可查数据
 "get_qhkc_index"  # 获取奇货可查-指数-数值数据
 "get_qhkc_index_profit_loss"  # 获取奇货可查-指数-累计盈亏数据
 "get_qhkc_index_trend"  # 获取奇货可查-指数-大资金动向数据
 "get_qhkc_fund_bs"  # 获取奇货可查-资金-净持仓分布数据
 "get_qhkc_fund_position"  # 获取奇货可查-资金-总持仓分布数据
 "get_qhkc_fund_position_change"  # 获取奇货可查-资金-净持仓变化分布数据
 "get_qhkc_tool_foreign"  # 获取奇货可查-工具-外盘比价数据
 "get_qhkc_tool_gdp"  # 获取奇货可查-工具-各地区经济数据
 # 中国银行间市场交易所数据
 "get_bond_bank"  # 获取中国银行间市场交易商协会-债券数据
 # 智道智科-私募指数数据
 "get_zdzk_fund_index"  # 获取智道智科-私募指数数据
 # 提供英为财情数据接口
 "get_country_index"  # 提供英为财情-股票指数-全球股指与期货指数数据
 "get_country_bond"  # 提供英为财情-债券数据-全球政府债券行情与收益率数据
 # 交易所商品期权数据
 "get_dce_option_daily"  # 提供大连商品交易所商品期权数据
 "get_czce_option_daily"  # 提供郑州商品交易所商品期权数据
 "get_shfe_option_daily"  # 提供上海期货交易所商品期权数据
 # 中国银行间市场债券行情数据
 "get_bond_market_quote"  # 债券市场行情-现券市场成交行情数据
 "get_bond_market_trade"  # 债券市场行情-现券市场做市报价数据
 # 外汇
 "get_fx_spot_quote"  # 人民币外汇即期报价数据
 "get_fx_swap_quote"  # 人民币外汇远掉报价数据
 "get_fx_pair_quote"  # 外币对即期报价数据
 # 商品
 "get_sector_futures"  # 全球商品数据数据
 # 宏观-欧洲
 "get_euro_interest_rate"  # 欧洲央行决议报告
 # 宏观-主要机构
 "get_cons_gold_amount"  # 全球最大黄金ETF—SPDR Gold Trust持仓报告-总价值
 "get_cons_gold_change"  # 全球最大黄金ETF—SPDR Gold Trust持仓报告-增持/减持
 "get_cons_gold_volume"  # 全球最大黄金ETF—SPDR Gold Trust持仓报告-总库存
 "get_cons_opec_month"  # 欧佩克报告-差异
 "get_cons_opec_near_change"  # 欧佩克报告-月份
 "get_cons_silver_amount"  # 全球最大白银ETF--iShares Silver Trust持仓报告-总价值
 "get_cons_silver_change"  # 全球最大白银ETF--iShares Silver Trust持仓报告-增持/减持
 "get_cons_silver_volume"  # 全球最大白银ETF--iShares Silver Trust持仓报告-总库存
 # 期货-仓单有效期
 "get_receipt_date"  # 期货仓单有效期数据
 # 新浪财经-期货
 "futures_zh_spot"  # 获取新浪-国内期货实时行情数据
 "futures_hq_spot"  # 获取新浪-外盘期货实时行情数据
 # 交易所金融期权数据
 "get_finance_option"  # 提供上海证券交易所期权数据
 # 数字货币行情
 "get_js_dc_current"  # 提供主流数字货币行情数据接口
 # 股票-企业社会责任
 "stock_zh_a_scr_report"  # 企业社会责任数据
 # 美股-中国概念股行情和历史数据
 "stock_us_zh_spot"  # 中国概念股行情
 "stock_us_zh_daily"  # 中国概念股历史数据
 # 新浪财经-港股
 "stock_hk_spot"  # 获取港股的历史行情数据(包括前后复权因子)
 "stock_hk_daily"  # 获取港股的实时行情数据(也可以用于获得所有港股代码)
 # 新浪财经-美股
 "stock_us_name"  # 获得美股的所有股票代码
 "stock_us_spot"  # 获取美股行情报价
 "stock_us_daily"  # 获取美股的历史数据(包括前复权因子)
 # A+H股实时行情数据和历史行情数据
 "stock_zh_ah_spot"  # 获取 A+H 股实时行情数据(延迟15分钟)
 "stock_zh_ah_daily"  # 获取 A+H 股历史行情数据(日频)
 "stock_zh_ah_name"  # 获取 A+H 股所有股票代码
 # A股实时行情数据和历史行情数据
 "stock_zh_a_spot"  # 获取 A 股实时行情数据
 "stock_zh_a_daily"  # 获取 A 股历史行情数据(日频)
 # 科创板实时行情数据和历史行情数据
 "stock_zh_kcb_spot"  # 获取科创板实时行情数据
 "stock_zh_kcb_daily"  # 获取科创板历史行情数据(日频)
 # 银保监分局本级行政处罚数据
 "bank_fjcf_table_detail"  # 获取银保监分局本级行政处罚-信息公开表
 # 已实现波动率数据
 "article_oman_rv"  # O-MAN已实现波动率
 "article_rlab_rv"  # Risk-Lab已实现波动率
 # FF多因子模型数据
 "ff_crr"  # FF当前因子
 # 指数实时行情和历史行情
 "stock_zh_index_daily"  # 股票指数历史行情数据
 "stock_zh_index_spot"  # 股票指数实时行情数据
 # 股票分笔数据
 "stock_zh_a_tick"  # A 股票分笔行情数据(近2年)
 # Websocket 实时监控
 "watch"  # 监控外汇实时价格
 # 世界各地区日出和日落数据-日
 "weather_daily"  # 每日日出和日落数据
 # 世界各地区日出和日落数据-月
 "weather_monthly"  # 每月日出和日落数据
 # 河北空气质量数据(期货-钢铁)
 "air_hebei"  # 河北空气质量数据
 # 南华期货-南华指数-波动率指数
 "nh_volatility_index"  # 波动率指数
 # 南华期货-南华指数-价格指数
 "nh_price_index"  # 价格指数
 # 南华期货-南华指数-收益率指数
 "nh_return_index"  # 收益率指数
 # 经济政策不确定性(EPU)指数
 "article_epu_index"  # 主要国家和地区的经济政策不确定性(EPU)指数
 # 微博指数
 "weibo_index"  # 获取3个月内的微博指数
 # 百度指数
 "baidu_search_index"  # 获取百度搜索指数
 "baidu_info_index"  # 获取百度资讯指数
 "baidu_media_index"  # 获取百度媒体指数
 # 谷歌指数
 "google_index"  # 获取谷歌趋势指数
 # 申万行业指数
 "sw_index_spot"  # 获取申万一级实时行情
 "sw_index_cons"  # 获取申万一级板块成份
 "sw_index_daily"  # 获取申万一级历史行情
 "sw_index_daily_indicator"  # 获取申万一级历史行情指标
 # 空气质量
 "air_all_city"  # 获取所有城市天气
 "air_city_list"  # 获取城市列表
 "air_daily"  # 获取每日天气
 "air_hourly"  # 获取每小时天气
 # 财富世界五百强公司
 "fortune_rank"  # 获取财富世界500强公司历年排名
 # 中国证券投资基金业协会-信息公示
 "amac_member_info" # 中国证券投资基金业协会-信息公示-会员信息-会员机构综合查询
 "amac_person_org_list" # 中国证券投资基金业协会-信息公示-从业人员信息-基金从业人员资格注册信息
 "amac_person_org_list_ext" # 中国证券投资基金业协会-信息公示-从业人员信息-基金从业人员资格注册外部公示信息
 "amac_manager_info" # 中国证券投资基金业协会-信息公示-私募基金管理人公示-私募基金管理人综合查询
 "amac_manager_classify_info" # 中国证券投资基金业协会-信息公示-私募基金管理人公示-私募基金管理人分类公示
 "amac_member_sub_info" # 中国证券投资基金业协会-信息公示-私募基金管理人公示-证券公司私募基金子公司管理人信息公示
 "amac_fund_info" # 中国证券投资基金业协会-信息公示-基金产品-私募基金管理人基金产品
 "amac_securities_info" # 中国证券投资基金业协会-信息公示-基金产品-证券公司集合资管产品公示
 "amac_aoin_info" # 中国证券投资基金业协会-信息公示-基金产品-证券公司直投基金
 "amac_fund_sub_info" # 中国证券投资基金业协会-信息公示-基金产品公示-证券公司私募投资基金
 "amac_fund_account_info" # 中国证券投资基金业协会-信息公示-基金产品公示-基金公司及子公司集合资管产品公示
 "amac_fund_abs" # 中国证券投资基金业协会-信息公示-基金产品公示-资产支持专项计划
 "amac_futures_info" # 中国证券投资基金业协会-信息公示-基金产品公示-期货公司集合资管产品公示
 "amac_manager_xxgs_hmd" # 中国证券投资基金业协会-信息公示-诚信信息-违反自律规则黑名单
 "amac_manager_xxgs_jlcf" # 中国证券投资基金业协会-信息公示-诚信信息-纪律处分
 "amac_manager_xxgs_cxdj" # 中国证券投资基金业协会-信息公示-诚信信息-撤销管理人登记的名单
 "amac_manager_cancelled_info" # 中国证券投资基金业协会-信息公示-诚信信息-已注销私募基金管理人名单
 # 全国银行间同业拆借中心-市场数据-市场行情-外汇市场行情
 "fx_spot_quote"  # 市场行情-外汇市场行情-人民币外汇即期报价
 "fx_swap_quote"  # 市场行情-债券市场行情-人民币外汇远掉报价
 "fx_pair_quote"  # 市场行情-债券市场行情-外币对即期报价
 # 能源-碳排放权
 "energy_carbon"  # 北京市碳排放权电子交易平台-北京市碳排放权公开交易行情
 # 电影-实时票房
 "movie_board"  # 获取上映影片实时票房数据
 # 生活成本
 "cost_living"  # 获取世界各大城市生活成本数据
 # 商品现货价格指数
 "spot_goods"  # 获取商品现货价格指数
 # 中国宏观杠杆率
 "macro_cnbs"  # 获取中国宏观杠杆率数据
 # 金融期权
 "option_finance_board"  # 获取金融期权数据
 # 期货连续合约
 "futures_main_sina"  # 获取新浪期货连续合约的历史数据
 # 倒闭公司数据
 "death_company"  # 获取2014至今倒闭公司名单
 # 独角兽公司数据
 "nicorn_company"  # 获取独角兽公司名单
 # 千里马公司数据
 "maxima_company"  # 获取千里马公司名单
 # 机构调研数据
 "stock_em_jgdy_tj"  # 获取机构调研数据-统计
 "stock_em_jgdy_detail"  # 获取机构调研数据-详细
 # 股权质押数据
 "stock_em_gpzy_profile"  # 获取股权质押市场概况
 "stock_em_gpzy_pledge_ratio"  # 获取上市公司质押比例
 "stock_em_gpzy_pledge_ratio_detail"  # 获取重要股东股权质押明细
 "stock_em_gpzy_distribute_statistics_company"  # 获取质押机构分布统计-证券公司
 "stock_em_gpzy_distribute_statistics_bank"  # 获取质押机构分布统计-银行
 "stock_em_gpzy_industry_data"  # 获取上市公司质押比例-行业数据
 # 商誉专题数据
 "stock_em_sy_profile"  # 获取A股商誉市场概况
 "stock_em_sy_yq_list"  # 获取商誉减值预期明细
 "stock_em_sy_jz_list"  # 获取个股商誉减值明细
 "stock_em_sy_list"  # 获取个股商誉明细
 "stock_em_sy_hy_list"  # 获取行业商誉
 # 股票账户统计数据
 "stock_em_account"  # 获取股票账户统计数据
 # 交易法门-工具接口-套利分析
 "jyfm_tools_futures_spread"  # 交易法门-工具-套利分析-跨期价差(自由价差)
 "jyfm_tools_futures_ratio"  # 交易法门-工具-套利分析-自由价比
 "jyfm_tools_futures_customize"  # 交易法门-工具-套利分析-多腿组合
 "jyfm_exchange_symbol_dict"  # 交易法门-交易所-品种字典
 "jyfm_tools_position_detail"  # 交易法门-工具-持仓分析-期货分析
 "jyfm_tools_position_seat"  # 交易法门-工具-持仓分析-持仓分析
 # 交易法门-工具接口-交易规则
 "jyfm_tools_receipt_expire_info"  # 交易法门-工具-交易规则-仓单有效期
 "jyfm_tools_position_limit_info"  # 交易法门-工具-交易规则-限仓规定
 # 交易法门-数据接口-农产品
 "jyfm_data_cocking_coal"  # 交易法门-数据-黑色系-焦煤
 "jyfm_data_palm"  # 交易法门-数据-农产品-棕榈
 "jyfm_data_soybean_meal"  # 交易法门-数据-农产品-豆粕
 "jyfm_data_sugar"  # 交易法门-数据-农产品-白糖
 "jyfm_data_usa_bean"  # 交易法门-数据-农产品-美豆
 "jyfm_data_soybean_oil"  # 交易法门-数据-农产品-豆油
 # 股票指数-成份股
 "index_stock_cons"  # 股票指数-成份股-最新成份股获取
 "index_stock_info"  # 股票指数-成份股-所有可以获取的指数表
 # 义乌小商品指数
 "index_yw"  # 获取义乌小商品指数
 # 交易法门-工具-期限分析
 "jyfm_tools_futures_basis_daily"  # 交易法门-工具-期限分析-基差日报
 "jyfm_tools_futures_basis_analysis"  # 交易法门-工具-期限分析-基差分析
 "jyfm_tools_futures_basis_structure"  # 交易法门-工具-期限分析-期限结构
 "jyfm_tools_futures_basis_rule"  # 交易法门-工具-期限分析-价格季节性
 # 交易法门-工具-资讯汇总
 "jyfm_tools_research_query"  # 交易法门-工具-资讯汇总-研报查询
 "jyfm_tools_trade_calendar"  # 交易法门-工具-资讯汇总-交易日历
 # 交易法门-工具-资金分析
 "jyfm_tools_position_fund"  # 交易法门-工具-资金分析-资金流向
 # 交易法门-工具-仓单分析
 "jyfm_tools_warehouse_receipt_daily"  # 交易法门-工具-仓单分析-仓单日报
 "jyfm_tools_warehouse_receipt_query"  # 交易法门-工具-仓单分析-仓单查询
 "jyfm_tools_warehouse_receipt_ratio"  # 交易法门-工具-仓单分析-虚实盘比查询
 # 世界银行间拆借利率
 "rate_interbank"  #  银行间拆借利率
 # 主要央行利率
 "macro_bank_usa_interest_rate"  # 美联储利率决议报告
 "macro_bank_euro_interest_rate"  # 欧洲央行决议报告
 "macro_bank_newzealand_interest_rate"  # 新西兰联储决议报告
 "macro_bank_china_interest_rate"  # 中国央行决议报告
 "macro_bank_switzerland_interest_rate"  # 瑞士央行决议报告
 "macro_bank_english_interest_rate"  # 英国央行决议报告
 "macro_bank_australia_interest_rate"  # 澳洲联储决议报告
 "macro_bank_japan_interest_rate"  # 日本央行决议报告
 "macro_bank_russia_interest_rate"  # 俄罗斯央行决议报告
 "macro_bank_india_interest_rate"  # 印度央行决议报告
 "macro_bank_brazil_interest_rate"  # 巴西央行决议报告
 # 中国
 "macro_china_gdp_yearly"  # 金十数据中心-经济指标-中国-国民经济运行状况-经济状况-中国GDP年率报告
 "macro_china_cpi_yearly"  # 金十数据中心-经济指标-中国-国民经济运行状况-物价水平-中国CPI年率报告
 "macro_china_cpi_monthly"  # 金十数据中心-经济指标-中国-国民经济运行状况-物价水平-中国CPI月率报告
 "macro_china_ppi_yearly"  # 金十数据中心-经济指标-中国-国民经济运行状况-物价水平-中国PPI年率报告
 "macro_china_exports_yoy"  # 金十数据中心-经济指标-中国-贸易状况-以美元计算出口年率报告
 "macro_china_imports_yoy"  # 金十数据中心-经济指标-中国-贸易状况-以美元计算进口年率
 "macro_china_trade_balance"  # 金十数据中心-经济指标-中国-贸易状况-以美元计算贸易帐(亿美元)
 "macro_china_industrial_production_yoy"  # 金十数据中心-经济指标-中国-产业指标-规模以上工业增加值年率
 "macro_china_pmi_yearly"  # 金十数据中心-经济指标-中国-产业指标-官方制造业PMI
 "macro_china_cx_pmi_yearly"  # 金十数据中心-经济指标-中国-产业指标-财新制造业PMI终值
 "macro_china_cx_services_pmi_yearly"  # 金十数据中心-经济指标-中国-产业指标-财新服务业PMI
 "macro_china_non_man_pmi"  # 金十数据中心-经济指标-中国-产业指标-中国官方非制造业PMI
 "macro_china_fx_reserves_yearly"  # 金十数据中心-经济指标-中国-金融指标-外汇储备(亿美元)
 "macro_china_m2_yearly"  # 金十数据中心-经济指标-中国-金融指标-M2货币供应年率
 "macro_china_shibor_all"  # 金十数据中心-经济指标-中国-金融指标-上海银行业同业拆借报告
 "macro_china_hk_market_info"  # 金十数据中心-经济指标-中国-金融指标-人民币香港银行同业拆息
 "macro_china_daily_energy"  # 金十数据中心-经济指标-中国-其他-中国日度沿海六大电库存数据
 "macro_china_rmb"  # 金十数据中心-经济指标-中国-其他-中国人民币汇率中间价报告
 "macro_china_market_margin_sz"  # 金十数据中心-经济指标-中国-其他-深圳融资融券报告
 "macro_china_market_margin_sh"  # 金十数据中心-经济指标-中国-其他-上海融资融券报告
 "macro_china_au_report"  # 金十数据中心-经济指标-中国-其他-上海黄金交易所报告
 "macro_china_ctci"  # 发改委-中国电煤价格指数-全国综合电煤价格指数
 "macro_china_ctci_detail"  # 发改委-中国电煤价格指数-各价区电煤价格指数
 "macro_china_ctci_detail_hist"  # 发改委-中国电煤价格指数-历史电煤价格指数
 # 美国
 "macro_usa_gdp_monthly"  # 金十数据中心-经济指标-美国-经济状况-美国GDP
 "macro_usa_cpi_monthly"  # 金十数据中心-经济指标-美国-物价水平-美国CPI月率报告
 "macro_usa_core_cpi_monthly"  # 金十数据中心-经济指标-美国-物价水平-美国核心CPI月率报告
 "macro_usa_personal_spending"  # 金十数据中心-经济指标-美国-物价水平-美国个人支出月率报告
 "macro_usa_retail_sales"  # 金十数据中心-经济指标-美国-物价水平-美国零售销售月率报告
 "macro_usa_import_price"  # 金十数据中心-经济指标-美国-物价水平-美国进口物价指数报告
 "macro_usa_export_price"  # 金十数据中心-经济指标-美国-物价水平-美国出口价格指数报告
 "macro_usa_lmci"  # 金十数据中心-经济指标-美国-劳动力市场-LMCI
 "macro_usa_unemployment_rate"  # 金十数据中心-经济指标-美国-劳动力市场-失业率-美国失业率报告
 "macro_usa_job_cuts"  # 金十数据中心-经济指标-美国-劳动力市场-失业率-美国挑战者企业裁员人数报告
 "macro_usa_non_farm"  # 金十数据中心-经济指标-美国-劳动力市场-就业人口-美国非农就业人数报告
 "macro_usa_adp_employment"  # 金十数据中心-经济指标-美国-劳动力市场-就业人口-美国ADP就业人数报告
 "macro_usa_core_pce_price"  # 金十数据中心-经济指标-美国-劳动力市场-消费者收入与支出-美国核心PCE物价指数年率报告
 "macro_usa_real_consumer_spending"  # 金十数据中心-经济指标-美国-劳动力市场-消费者收入与支出-美国实际个人消费支出季率初值报告
 "macro_usa_trade_balance"  # 金十数据中心-经济指标-美国-贸易状况-美国贸易帐报告
 "macro_usa_current_account"  # 金十数据中心-经济指标-美国-贸易状况-美国经常帐报告
 "macro_usa_rig_count"  # 金十数据中心-经济指标-美国-产业指标-制造业-贝克休斯钻井报告
 # 金十数据中心-经济指标-美国-产业指标-制造业-美国个人支出月率报告
 "macro_usa_ppi"  # 金十数据中心-经济指标-美国-产业指标-制造业-美国生产者物价指数(PPI)报告
 "macro_usa_core_ppi"  # 金十数据中心-经济指标-美国-产业指标-制造业-美国核心生产者物价指数(PPI)报告
 "macro_usa_api_crude_stock"  # 金十数据中心-经济指标-美国-产业指标-制造业-美国API原油库存报告
 "macro_usa_pmi"  # 金十数据中心-经济指标-美国-产业指标-制造业-美国Markit制造业PMI初值报告
 "macro_usa_ism_pmi"  # 金十数据中心-经济指标-美国-产业指标-制造业-美国ISM制造业PMI报告
 "macro_usa_nahb_house_market_index"  # 金十数据中心-经济指标-美国-产业指标-房地产-美国NAHB房产市场指数报告
 "macro_usa_house_starts"  # 金十数据中心-经济指标-美国-产业指标-房地产-美国新屋开工总数年化报告
 "macro_usa_new_home_sales"  # 金十数据中心-经济指标-美国-产业指标-房地产-美国新屋销售总数年化报告
 "macro_usa_building_permits"  # 金十数据中心-经济指标-美国-产业指标-房地产-美国营建许可总数报告
 "macro_usa_exist_home_sales"  # 金十数据中心-经济指标-美国-产业指标-房地产-美国成屋销售总数年化报告
 "macro_usa_house_price_index"  # 金十数据中心-经济指标-美国-产业指标-房地产-美国FHFA房价指数月率报告
 "macro_usa_spcs20" # 金十数据中心-经济指标-美国-产业指标-房地产-美国S&P/CS20座大城市房价指数年率报告
 "macro_usa_pending_home_sales"  # 金十数据中心-经济指标-美国-产业指标-房地产-美国成屋签约销售指数月率报告
 "macro_usa_cb_consumer_confidence"  # 金十数据中心-经济指标-美国-领先指标-美国谘商会消费者信心指数报告
 "macro_usa_nfib_small_business" # 金十数据中心-经济指标-美国-领先指标-美国NFIB小型企业信心指数报告
 "macro_usa_michigan_consumer_sentiment" # 金十数据中心-经济指标-美国-领先指标-美国密歇根大学消费者信心指数初值报告
 "macro_usa_eia_crude_rate"  # 金十数据中心-经济指标-美国-其他-美国EIA原油库存报告
 "macro_usa_initial_jobless"  # 金十数据中心-经济指标-美国-其他-美国初请失业金人数报告
 "macro_usa_crude_inner"  # 金十数据中心-经济指标-美国-其他-美国原油产量报告
 "macro_usa_crude_state"  # 金十数据中心-经济指标-美国-其他-美国本土48州原油产量
 "macro_usa_crude_alaska"  # 金十数据中心-经济指标-美国-其他-美国阿拉斯加州原油产量
 # 更新宏观数据
 "macro_cons_gold_volume"  # 全球最大黄金ETF—SPDR Gold Trust持仓报告
 "macro_cons_gold_change"  # 全球最大黄金ETF—SPDR Gold Trust持仓报告
 "macro_cons_gold_amount"  # 全球最大黄金ETF—SPDR Gold Trust持仓报告
 "macro_cons_silver_volume"  # 全球最大白银ETF--iShares Silver Trust持仓报告
 "macro_cons_silver_change"  # 全球最大白银ETF--iShares Silver Trust持仓报告
 "macro_cons_silver_amount"  # 全球最大白银ETF--iShares Silver Trust持仓报告
 "macro_cons_opec_near_change"  # 欧佩克报告-变动
 "macro_cons_opec_month"  # 欧佩克报告-月度
 # 新型冠状病毒数据接口
 "epidemic_163"  # 新型冠状病毒-网易
 "epidemic_dxy"  # 新型冠状病毒-丁香园
```

## 3. 案例演示

### 3.1 获取展期收益率

代码:

```python
import akshare as ak
ak.get_roll_yield_bar(type_method="date", var="RB", start_day="20180618", end_day="20180718", plot=True)
```

结果显示: 日期, 展期收益率, 最近合约, 下一期合约

```
            roll_yield near_by deferred
2018-06-19    0.191289  RB1810   RB1901
2018-06-20    0.192123  RB1810   RB1901
2018-06-21    0.183304  RB1810   RB1901
2018-06-22    0.190642  RB1810   RB1901
2018-06-25    0.194838  RB1810   RB1901
2018-06-26    0.204314  RB1810   RB1901
2018-06-27    0.213667  RB1810   RB1901
2018-06-28    0.211701  RB1810   RB1901
2018-06-29    0.205892  RB1810   RB1901
2018-07-02    0.224809  RB1810   RB1901
2018-07-03    0.229198  RB1810   RB1901
2018-07-04    0.222853  RB1810   RB1901
2018-07-05    0.247187  RB1810   RB1901
2018-07-06    0.261259  RB1810   RB1901
2018-07-09    0.253283  RB1810   RB1901
2018-07-10    0.225832  RB1810   RB1901
2018-07-11    0.210659  RB1810   RB1901
2018-07-12    0.212805  RB1810   RB1901
2018-07-13    0.170282  RB1810   RB1901
2018-07-16    0.218066  RB1810   RB1901
2018-07-17    0.229768  RB1810   RB1901
2018-07-18    0.225529  RB1810   RB1901
```

### 3.2 获取私募指数数据

代码:

```python
import akshare as ak
ak.zdzk_fund_index(index_type=32, plot=True)
```

结果显示: 日期, 指数数值

```
2014-12-26    1000.000000
2015-01-02     985.749098
2015-01-09    1032.860242
2015-01-16    1039.978586
2015-01-23    1046.235945
                 ...     
2019-08-23    1390.816835
2019-08-30    1397.684642
2019-09-06    1402.711847
2019-09-13    1401.723599
2019-09-20    1386.570103
```
 