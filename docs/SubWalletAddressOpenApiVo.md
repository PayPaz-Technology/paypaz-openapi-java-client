

# SubWalletAddressOpenApiVo

企业子用户钱包地址实体类  用于存储和管理子用户的钱包地址信息  对应数据库表：tb_sub_wallet_address

## Properties

| Name | Type | Description | Notes |
|------------ | ------------- | ------------- | -------------|
|**id** | **String** | 主键ID |  [optional] |
|**userId** | **String** | 用户ID  主账号用户的标识符 |  [optional] |
|**tokenId** | **String** | 币种ID  例如：USDT，USDC等 |  [optional] |
|**chainId** | **String** | chainId  例如：BNB，TRON |  [optional] |
|**address** | **String** | 钱包地址  区块链上的钱包地址，用于接收充值 |  [optional] |
|**createdAt** | **String** | 创建时间  记录创建的时间戳（毫秒） |  [optional] |
|**updatedAt** | **String** | 更新时间  记录最后更新的时间戳（毫秒） |  [optional] |
|**tag** | **String** | 标签  某些币种（如XRP、XLM等）需要的额外标识符 |  [optional] |
|**subUserId** | **String** | 子用户ID  企业-子用户的ID，标识具体的子账号 |  [optional] |



