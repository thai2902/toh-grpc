GO_OUT_DIR=./server
JS_OUT_DIR=./client/src/app
protoc proto/hero.proto --go_out=${GO_OUT_DIR} --ts_out="service=grpc-node:${JS_OUT_DIR}" --js_out="import_style=commonjs,binary:${JS_OUT_DIR}"