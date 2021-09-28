# Liquity B-Protocol Implementation Server

This server hosts the B-Protocol implemented Liqiuty Frontend

## Steps to Take

1. Clone/fork [AngelDAO/Liquity-B-Protocol-Integration](https://github.com/AngelDao/Liquity-b-protocol-Frontend).

2. Go to repo in terminal, then navigate to `/dev` and run `yarn` followed by `yarn build`. This will output a `bulid/` directory in `./dev/packages/dev-frontend/`

3. Copy contents of the build directory `build/*` and paste it into this repos `public` directory.

4. Clone/fork [B-Protocol/dev](https://github.com/backstop-protocol/dev)

5. Go to repo in terminal, then navigate to `/dev` and run `yarn`

6. Navigate to `./dev/packages/dev-frontend/` and change the value for the `homepage` in `package.json` to be:

```
"homepage": "/b-protocol"
```

7. Navigate back to `./dev` and run `yarn build`. This will output a `bulid/` directory in `./dev/packages/dev-frontend/`

8. Rename the `build/` directory to `b-protocol/` and paste directory into `public` in this repo

9. Test it works by running `node server.js` or `yarn start`
