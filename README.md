# LuciExample

Demo [Angular CLI](https://github.com/angular/angular-cli) (version 8.0.1) project to show LUCI SCSS build issue.

Just installed LUCI and added a reference to `src/styles.scss`

```
npm install
npm run build
```

## Error

```
ERROR in ./src/styles.scss (./node_modules/@angular-devkit/build-angular/src/angular-cli-files/plugins/raw-css-loader.js!./node_modules/postcss-loader/src??embedded!./node_modules/sass-loader/lib/loader.js??ref--13-3!./src/styles.scss)
Module build failed (from ./node_modules/sass-loader/lib/loader.js):

    background-image: url('data:image/svg+xml;utf8,
                                                  ^
      Expected '.
   ╷
20 │     background-image: url('data:image/svg+xml;utf8,
   │                                                    ^
   ╵
  node_modules/@netapp/luci/components/table/table.scss 20:52  root stylesheet
  node_modules/@netapp/luci/styles/luci.scss 25:9              @import
  stdin 2:9                                                    root stylesheet
      in /path-to-repo/luci-example/node_modules/@netapp/luci/components/table/table.scss (line 20, column 52)
```
