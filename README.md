[![Build Status](https://travis-ci.org/telemark/portalen-tasks.svg?branch=master)](https://travis-ci.org/telemark/portalen-tasks)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](https://github.com/feross/standard)
# portalen-tasks

[![Greenkeeper badge](https://badges.greenkeeper.io/telemark/portalen-tasks.svg)](https://greenkeeper.io/)
All-in-one solution for tasks and portalen

## API
Exposes API. Auth header with jwt

### /user/{userId}
Returns tasks for given user

```bash
$ curl -v -H 'Authorization: your.very.long.jwt' http://localhost:8000/user/mememe 
```

## Docker
```bash
 docker run -d --env-file ./tasks.env -p 8000:8000 --name portalen-tasks telemark/portalen-tasks
```

## License
[MIT](LICENSE)
