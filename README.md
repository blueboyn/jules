curl -k -X POST `
  https://127.0.0.1:57412/config/v1/project/channels/Channel1/devices/Device1/tags `
  -H "Content-Type: application/json" `
  -u "Administrator:" `
  -d '{
    "common.ALLTYPES_NAME": "NewTag001",
    "servermain.TAG_ADDRESS": "D100",
    "servermain.TAG_DATA_TYPE": 5,
    "servermain.TAG_READ_WRITE_ACCESS": 1,
    "servermain.TAG_SCAN_RATE_MILLISECONDS": 1000
  }'
curl -k -X POST https://127.0.0.1:57412/config/v1/project/channels/Channel1/devices/Device1/tags -H "Content-Type: application/json" -u Administrator: -d "{\"common.ALLTYPES_NAME\":\"NewTag001\",\"servermain.TAG_ADDRESS\":\"D100\",\"servermain.TAG_DATA_TYPE\":5,\"servermain.TAG_READ_WRITE_ACCESS\":1}"

"# jules dev version"