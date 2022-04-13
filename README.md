# grpc-up-and-running
Following alowg with the gRPC: Up and Running book

## Generate

### Messages
```bash
protoc -I ecommerce ecommerce/product_info.proto \
--go_out=./ecommerce \
--go_opt=paths=source_relative
```

### Services
```bash
protoc -I ecommerce ecommerce/product_info.proto \
--go-grpc_out=./ecommerce \
--go-grpc_opt=paths=source_relative
```

## Acknowledgement

- gRPC: Up and Running by Kasun Indrasiri and Danesh Kuruppu (O’Reilly). Copyright 2020 Kasun Indrasiri and Danesh Kuruppu, 978-1-492-05833-5.
- [Code samples](https://github.com/grpc-up-and-running/samples)