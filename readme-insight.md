### How to publish to Nexus

```
npm config set @ni:registry https://nexus.infra.nagra-insight.com/repository/npm-releases/
npm config set _auth $(echo -n insight-rw:$(gopass show nexus/insight-rw) | openssl base64)
yarn build publish
```

### How to install it

```
npm install --global "@ni/renovate@31.2.3-ni-build.2"
```
