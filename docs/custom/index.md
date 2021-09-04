<p align="center">
  <a  href="https://github.com/NoeCruzMW/zpy-flask-msc-docs"><img width="150" src="https://lh3.googleusercontent.com/a-/AOh14GjLO5qYYR5nQl5hgavUKz4Dv3LVzWDvGtV4xNam=s600-k-no-rp-mo" alt="Zurck'z"></a>
</p>
<p align="center">
    <em>ZPy Flask MSC, easy to learn, fast to code, ready for production</em>
</p>
<p align="center"></p>

---
# CUSTOM Module

> Zurck'z  Py Flask Micro Services Core

This package contains some helpers features for python microservices using Flask framework

ZPy need of giants, include
- pycryptodome
- Flask
- marshmallow
- cx-Oracle

## Requirements

- Python 3.6+
- Boto 3+
- Oracle clinet


## Installation


Use the package manager [pip](https://pip.pypa.io/en/stable/) to install py flask micro service core .

```bash
pip install trade-py-core
```

## Basic Usage

```python
#Define api
@api(base='/v1', config=config,hooks=hk,middlewares=mw)
def create_api():
    #Define all dependencies for enterprise resources
    service = CompanyService(repository=CompanyRepositoryImpl(db))
    #Set all supported resource for this web service.
    return \
    [
        ZResource('/', CompanyResource,service=service),
        ...
    ]
```

## Features

Contains some helper modules.
### Custom 

This module contains exactly plugins for use Oracle and AWS System manager with specific models.

[See More](../)


## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[MIT](https://choosealicense.com/licenses/mit/)

## Authors
[Noé Cruz](noe.isc20@gmail.com)