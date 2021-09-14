# PostgreSQL GitHub Action
This action ensures that a postgresql server is running.

This project is a fork of https://github.com/Harmon758/postgresql-action, with the defaults changed to our defaults
## Usage

```yaml
steps:
- uses: quickpay/postgresql-action@v2
  with:
    # the version of postgres server to run as
    # default is 11
    postgresql version: "11"

    # the name of the database in question
    # default is "backends_test"
    postgresql db: "backends_test"

    # the name of the user with superuser powers that gonna be created
    # default is "backends_u"
    postgresql user: "backends_u"

    # the password of the super user
    # default is "abc"
    postgresql password: "abc"
```

This project is almost always used in conjunction with [QuickPay/quickpay-base-action](https://github.com/QuickPay/quickpay-base-action)'s postgres mode