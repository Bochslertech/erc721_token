## Tests Locallt

- Download and Install [vessel](https://github.com/dfinity/vessel)
- run `vessel install`
- run `dfx start --clean`
- run `dfx deploy erc721 --argument '(principal "'$(dfx identity get-principal)'")'`

## NFT metadata
```json
{
	"url": "https://pgi7h-uqaaa-aaaao-ae6ha-cai.raw.ic0.app/file/0.png",//NFT主资产地址，不可空
	"thumb": "https://pgi7h-uqaaa-aaaao-ae6ha-cai.raw.ic0.app/file/0_thumb.jpeg",//NFT资产缩略图，可空
	"name": "NEPTUNE CARD #0",
	"mimeType": "image",//资产类型，目前支持image/video/3dmodel 三种类型，默认image
	"attributes": [{//属性，可空
		"trait_type": "listing referrer ",
		"value": "No"
	}, {
		"trait_type": "vip market-maker",
		"value": "Yes"
	}]
}
```