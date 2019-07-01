# vcnd
Testing CodeNotary vcn as deamon

## Usage

After starting the server:
```
docker-compose build --no-cache
docker-compose up -d
```

Then, in order to test that everything is working, open http://localhost:9000/verify/a7c1882a49daba3855bf48c4ac208405e3489acccef6aaa9c79f72b0b55cf6ba 

### Verify endpoint

*Path*

`/verify/<hash>`

*Query params*

- `keys` comma-separted list of signers' keys to verify against
- `org` organization ID to verify against
> If `org` is present, `keys` will be ignored.

