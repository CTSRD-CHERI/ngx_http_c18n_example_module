# ngx_http_c18n_example_module

Custom nginx module for reponsding to a POST request.

## Build

```
auto/configure --with-cc-opt='-Wno-cheri-provenance' --with-compat --add-dynamic-module=src/ngx_http_c18n_example_module --with-debug
gmake modules
```

## Configure

```
location /test {
  ...
  print_c18n_example;
}
```
