# solr8-nested-documents
Use nested documents with Solr 8

# Solr Schema Configuration
- Nested Schema
- Only one dynamic field is defined (`*_str`)

# How to run
Run the container
```
docker run --rm --volume="$PWD/cores:/var/solr/data" -it -p 8983:8983 --name solr-example solr:8.2.0
```

Stop container
```
docker stop solr-example
```

Restart container
```
docker restart solr-example
```

View logs
```
docker logs -f --tail=1000 solr-example
```

# How to test
Import the postman collection in `postman` folder.
More details in:
- [Index nested documents with Solr 8](https://lenguyenhaohiep.github.io/solr/Index-nested-documents-Solr-8/)
- [Search and Faceting on nested documents with Solr 8](https://lenguyenhaohiep.github.io/solr/search-facet-nested-documents/)
- [Use atomic update on nested document with Solr 8](https://lenguyenhaohiep.github.io/solr/atomic-update-nested-documents/)
