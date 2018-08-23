# node-addon-api Changelog

## 2018-07-19 Version 1.4.0 (Current), @NickNasso 

### Notable changes:

#### Documentation

- Numerous additions to the documentation, filling out coverage
  of API surface

#### API

- Add resource parameters to AsyncWorker constructor
- Add memory management feature

### Commits

* [[`7dc5ac8bc3`](https://github.com/nodejs/node-addon-api/commit/7dc5ac8bc3)] - **doc**: update metadata for release (Nicola Del Gobbo)
* [[`d68e86adb4`](https://github.com/nodejs/node-addon-api/commit/d68e86adb4)] - **doc**: Added documentation for PropertyDescriptor (Anisha Rohra) [#309](https://github.com/nodejs/node-addon-api/pull/309)
* [[`968a5f2000`](https://github.com/nodejs/node-addon-api/commit/968a5f2000)] - **doc**: Add documentation for ObjectReference.md (Anisha Rohra) [#307](https://github.com/nodejs/node-addon-api/pull/307)
* [[`908cdc314c`](https://github.com/nodejs/node-addon-api/commit/908cdc314c)] - **doc**: add `TypedArray` and `TypedArrayOf` (Kyle Farnung) [#305](https://github.com/nodejs/node-addon-api/pull/305)
* [[`2ff776ffe3`](https://github.com/nodejs/node-addon-api/commit/2ff776ffe3)] - backport node::Persistent (Gabriel Schulhof) [#300](https://github.com/nodejs/node-addon-api/pull/300)
* [[`98161970c9`](https://github.com/nodejs/node-addon-api/commit/98161970c9)] - Backport perf, crash and exception handling fixes (Gabriel Schulhof) [#295](https://github.com/nodejs/node-addon-api/pull/295)
* [[`dd1191e086`](https://github.com/nodejs/node-addon-api/commit/dd1191e086)] - **test**: fix asyncworker test so it runs on 6.x (Michael Dawson) [#298](https://github.com/nodejs/node-addon-api/pull/298)
* [[`11697fcecd`](https://github.com/nodejs/node-addon-api/commit/11697fcecd)] - **doc**: ArrayBuffer and Buffer documentation (Kyle Farnung) [#256](https://github.com/nodejs/node-addon-api/pull/256)
* [[`605aa2babf`](https://github.com/nodejs/node-addon-api/commit/605aa2babf)] - Add memory management feature (NickNaso) [#286](https://github.com/nodejs/node-addon-api/pull/286)
* [[`86be13a611`](https://github.com/nodejs/node-addon-api/commit/86be13a611)] - **doc**: Fix HandleScope docs (Ben Berman) [#287](https://github.com/nodejs/node-addon-api/pull/287)
* [[`90f92c4dc0`](https://github.com/nodejs/node-addon-api/commit/90f92c4dc0)] - **doc**: Update broken links in README.md (Hitesh Kanwathirtha) [#290](https://github.com/nodejs/node-addon-api/pull/290)
* [[`c2a620dc11`](https://github.com/nodejs/node-addon-api/commit/c2a620dc11)] - **doc**: Clarify positioning versus N-API (Michael Dawson) [#288](https://github.com/nodejs/node-addon-api/pull/288)
* [[`6cff890ee5`](https://github.com/nodejs/node-addon-api/commit/6cff890ee5)] - **doc**: Fix typo in docs (Ben Berman) [#284](https://github.com/nodejs/node-addon-api/pull/284)
* [[`7394bfd154`](https://github.com/nodejs/node-addon-api/commit/7394bfd154)] - **doc**: Fix typo in docs (Ben Berman) [#285](https://github.com/nodejs/node-addon-api/pull/285)
* [[`12b2cdeed3`](https://github.com/nodejs/node-addon-api/commit/12b2cdeed3)] - fix test files (Kyle Farnung) [#257](https://github.com/nodejs/node-addon-api/pull/257)
* [[`9ab6607242`](https://github.com/nodejs/node-addon-api/commit/9ab6607242)] - **doc**: Update Doc Version Number (joshgarde) [#277](https://github.com/nodejs/node-addon-api/pull/277)
* [[`e029a076c6`](https://github.com/nodejs/node-addon-api/commit/e029a076c6)] - **doc**: First pass at basic Node Addon API docs (Hitesh Kanwathirtha) [#268](https://github.com/nodejs/node-addon-api/pull/268)
* [[`74ff79717e`](https://github.com/nodejs/node-addon-api/commit/74ff79717e)] - **doc**: fix link to async\_worker.md (Michael Dawson)
* [[`5a63f45eda`](https://github.com/nodejs/node-addon-api/commit/5a63f45eda)] - **doc**: First step of error and async doc (NickNaso) [#272](https://github.com/nodejs/node-addon-api/pull/272)
* [[`9d38f61afb`](https://github.com/nodejs/node-addon-api/commit/9d38f61afb)] - **doc**: New Promise and Reference docs (Jim Schlight) [#243](https://github.com/nodejs/node-addon-api/pull/243)
* [[`43ff9fa836`](https://github.com/nodejs/node-addon-api/commit/43ff9fa836)] - **doc**: Updated Object documentation (Anisha Rohra) [#254](https://github.com/nodejs/node-addon-api/pull/254)
* [[`b197f7cc8b`](https://github.com/nodejs/node-addon-api/commit/b197f7cc8b)] - **doc**: minor typos (Nick Soggin) [#248](https://github.com/nodejs/node-addon-api/pull/248)
* [[`4b8918b352`](https://github.com/nodejs/node-addon-api/commit/4b8918b352)] - Add resource parameters to AsyncWorker constructor (Jinho Bang) [#253](https://github.com/nodejs/node-addon-api/pull/253)
* [[`1ecf7c19b6`](https://github.com/nodejs/node-addon-api/commit/1ecf7c19b6)] - **doc**: fix wrong link in readme (miloas) [#255](https://github.com/nodejs/node-addon-api/pull/255)
* [[`a750ed1932`](https://github.com/nodejs/node-addon-api/commit/a750ed1932)] - **release**: updates to metadata for next release (Michael Dawson)

## 2018-05-08 Version 1.3.0, @mhdawson

### Notable changes:

#### Documentation
- Added documentation for Scopes
- Added documentation for migration from NAN
- Update documentation to better explain the use of NODE_ADDON_API

#### API
- Implement data manipulation methods for dataview
- Use built-in N-API on Node.js >= 6.14.2
- Value
  - Added IsExternal()
  - IsObject() allow functions
- String
  - Fixed initialization of std::string to nullptr

#### Tests
- Fix test failures on linuxOne and AIX 
- Added basic tests for Scopes
- Fix MSVC warning C4244 in tests

### Commits

* [386c2aeb74] - test: remove dep on later C++ feature (Michael Dawson) https://github.com/nodejs/node-addon-api/pull/267
* [10697734da] - Use built-in N-API on Node.js >= 6.14.2 (Gabriel Schulhof)
* [75086da273] - test: add basic tests and doc for scopes (Michael Dawson) https://github.com/nodejs/node-addon-api/pull/250
* [341dbd25d5] - doc: update blurb explaining NODE_ADDON_API (Gabriel Schulhof) https://github.com/nodejs/node-addon-api/pull/251
* [cf6c93e4ee] - don't try to escape null (Michael Dawson) https://github.com/nodejs/node-addon-api/pull/245
* [15e4b35fc2] - test: fix MSVC warning C4244 in tests (Kyle Farnung) https://github.com/nodejs/node-addon-api/pull/236
* [7f3ca03b8e] - Create a doc for migration (Sampson Gao) https://github.com/nodejs/node-addon-api/pull/118
* [0a2177debe] - Fix test failures on linuxOne and AIX (Jinho Bang) https://github.com/nodejs/node-addon-api/pull/232
* [d567f4b6b5] - Added Napi::Value::IsExternal() (Eric Bickle) https://github.com/nodejs/node-addon-api/pull/227
* [1b0f0e004a] - Update node-gyp.md (Michele Campus) https://github.com/nodejs/node-addon-api/pull/226
* [faf19c4f7a] - Fixed initialization of std::string to nullptr (Eric Bickle) https://github.com/nodejs/node-addon-api/pull/228
* [9c4d321b57] - Implement data manipulation methods for dataview (Jinho Bang) https://github.com/nodejs/node-addon-api/pull/218
* [5a39fdca6f] - n-api: throw RangeError napi_create_typedarray() (Jinho Bang) https://github.com/nodejs/node-addon-api/pull/216
* [1376377202] - Make IsObject() allow functions (Jinho Bang) https://github.com/nodejs/node-addon-api/pull/217
* [673b59d319] - src: Initial implementation of DataView class (Jinho Bang) https://github.com/nodejs/node-addon-api/pull/205
* [0a899bf1c5] - doc: update indication of latest version (Michael Dawson) https://github.com/nodejs/node-addon-api/pull/211
* [17c74e5a5e] - n-api: RangeError in napi_create_dataview() (Jinho Bang) https://github.com/nodejs/node-addon-api/pull/214
* [4058a29989] - n-api: fix memory leak in napi_async_destroy() (Jinho Bang) https://github.com/nodejs/node-addon-api/pull/213

