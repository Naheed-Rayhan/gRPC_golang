## gRPC in Golang


This link is the inspiration. Shout out to the creator of this video. 
[Youtube](https://www.youtube.com/watch?v=gbrPMv_GuQY)


```bash
protoc \
--go_out=invoicer \
--go_opt=paths=source_relative \
--go-grpc_out=invoicer \
--go-grpc_opt=paths=source_relative \
invoicer.proto
```
