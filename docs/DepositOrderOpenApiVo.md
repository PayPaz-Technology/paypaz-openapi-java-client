

# DepositOrderOpenApiVo

充值订单OpenAPI响应VO

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | 充值订单ID |  [optional] |
|**orderNo** | **String** | 订单号 |  [optional] |
|**tokenId** | **String** | 币种ID |  [optional] |
|**chainId** | **String** | 链上币种ID |  [optional] |
|**quantity** | **String** | 充值数量 |  [optional] |
|**fee** | **String** | 手续费 |  [optional] |
|**netAmount** | **String** | 净入账金额 |  [optional] |
|**fromAddress** | **String** | 来源地址 |  [optional] |
|**walletAddress** | **String** | 钱包地址 |  [optional] |
|**txId** | **String** | 交易ID（区块链交易哈希） |  [optional] |
|**status** | **Integer** | 充值状态： 0: 初始化 INIT; 1: 完成 已到账; 2: 处理中 充值中; 3: 失败 |  [optional] |
|**createdAt** | **String** | 创建时间（毫秒时间戳） |  [optional] |
|**updatedAt** | **String** | 更新时间（毫秒时间戳） |  [optional] |
|**userId** | **String** | 用户ID（主账号） |  [optional] |
|**subUserId** | **String** | 子用户ID |  [optional] |



