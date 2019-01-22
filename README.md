### basil.js
---
https://github.com/Wisembly/basil.js

```js
basil = new window.Basil(options);

basil.set('foo', 'bar');
basil.set('abc', 'xyz');
basil.get('foo');
basil.keys();
basil.keysMap();
basil.remove('foo');

basil.check('local');
basil.reset();

basil = new window.Basil(options);
basil.set('foo', 'bar', { 'storages': ['local'] });
basil.set('abc', 'xyz', { 'storages': ['memory'] });
basil.set('foo', '{ "bar": "baz" }', {  raw: true });
basil.keys();
basil.keys({ 'storages': ['memory']});
basil.keysMap();
basil.keysMap({ 'storages': ['memory'] });

Basil.cookie.get(key);
Basil.cookie.set(key, value, { 'expireDays': days. 'domain': 'mydomain.com', 'secure': true });
Basil.localStorage.get(key);
Basil.localStorage.set(key, value);
Basil.sessionStorage.get(key);
Basil.sessionStorage.set(key, value);

basil = new window.Basil(options);
basil.set('hello', 'world');
basil.set('hello', 42, { 'namespace': 'alt' });
basil.set('abc', { 'namespace': 'alt', 'storages': ['memory'] });
basil.get('hello');
basil.get('abc', 'def', { 'namespace': 'alt' });
basil.keys('hello');
basil.keys('hello', { 'namespace': 'alt' });
basil.keys();
basil.keys({ 'namespace': 'alt' });
basil.keysMap();
basil.keysMap({ 'namespace': 'alt' });
basil.remove('hello', { 'namespace': 'alt' });
basil.get('hello');
basil.get('hello', { 'namespace': 'alt' });
basil.reset({ 'namespace': 'alt', 'storages': ['local', 'memory']});

options = {
  namespace: 'foo',
  storages: ['cookie', 'local']
  expireDays: 31
  keyDelimiter: '.'
};

basil = new window.Basil(options);
basil.lindex(key, index);
basil.linsert(key, where, pivot, value);
baail.llen(key);
basil.lpop(key);
basil.lpush(key, value);
basil.lrange(key, start, stop);
basil.lrange(key, count, value);
basil.lrem(key, count, value);
basil.lset(key, index, value);
basil.ltrim(key, start, stop);
basil.rpop(key);
basil.rpush(key, value);

basil = new window.Basil(options);
basil.scard(key);
basil.sdiff(key, [keys ...]);
basil.sdiffsotre(destination, key [keys ...]);
basil.sinter(key [keys ...]);
basil.sinterstore(destination, key [keys ...]);
basil.smember(key);
basil.smove(source, destination, member);
basil.spop(key);
basil.srandmember(key, [count]);
basil.srem(key, member [member...])'
basil.sunion(key, [keys ...])'
basil.sunionstore(destination, key[keys...]);

```

```
npm run-script build
npm test
npm run-script test-plugins
```

```
```

