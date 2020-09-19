# Budget_Tracker

## User Story

* As a user, I want to be able to add expenses and deposits to my budget with or without a connection. When entering transactions offline, they should populate the total when brought back online.

## Business Context

Giving users a fast and easy way to track their money is important, but allowing them to access that information anytime is even more important. Having offline functionality is paramount to our applications success.

## Installation

In order to run this budget locally, user will need to run the following command: sh npm install which will install the necessary package dependencies for the application.

## Usage

Using the Node command: npm start will initiate the application and uswe will be given series of questions to process the information.

## Video

Application functionality can be seen in the following video by using this link:
https://drive.google.com/file/d/15XMVlyCU2SPvLl8ANFIazJJJJVniuiO4/view

## Heroku App

Although the applicatioin is working locally I am unable to deploy through heroku.  

$ heroku logs
2020-09-19T18:09:24.167743+00:00 app[web.1]: npm ERR! This is probably not a problem with npm. There is likely additional logging output above.
2020-09-19T18:09:24.185146+00:00 app[web.1]:
2020-09-19T18:09:24.185687+00:00 app[web.1]: npm ERR! A complete log of this run can be found in:
2020-09-19T18:09:24.185930+00:00 app[web.1]: npm ERR!     /app/.npm/_logs/2020-09-19T18_09_24_169Z-debug.log
2020-09-19T18:09:24.297942+00:00 heroku[web.1]: Process exited with status 1
2020-09-19T18:09:24.338397+00:00 heroku[web.1]: State changed from starting to crashed
2020-09-19T18:21:53.000000+00:00 app[api]: Build started by user diego.resendez@yahoo.com
2020-09-19T18:22:19.170104+00:00 app[api]: Release v8 created by user diego.resendez@yahoo.com
2020-09-19T18:22:19.170104+00:00 app[api]: Deploy 55e05ec4 by user diego.resendez@yahoo.com
2020-09-19T18:22:19.666807+00:00 heroku[web.1]: State changed from crashed to starting
2020-09-19T18:22:21.000000+00:00 app[api]: Build succeeded
2020-09-19T18:22:23.132610+00:00 heroku[web.1]: Starting process with command `npm start`
2020-09-19T18:22:25.883237+00:00 app[web.1]:
2020-09-19T18:22:25.883264+00:00 app[web.1]: > budget-app@1.0.0 start /app
2020-09-19T18:22:25.883265+00:00 app[web.1]: > node server.js
2020-09-19T18:22:25.883265+00:00 app[web.1]:
2020-09-19T18:22:26.767065+00:00 app[web.1]: events.js:292
2020-09-19T18:22:26.767110+00:00 app[web.1]: throw er; // Unhandled 'error' event
2020-09-19T18:22:26.767111+00:00 app[web.1]: ^
2020-09-19T18:22:26.767111+00:00 app[web.1]:
2020-09-19T18:22:26.767112+00:00 app[web.1]: Error: listen EACCES: permission denied 0.0.0.0:1000
2020-09-19T18:22:26.767113+00:00 app[web.1]: at Server.setupListenHandle [as _listen2] (net.js:1296:21)
2020-09-19T18:22:26.767113+00:00 app[web.1]: at listenInCluster (net.js:1361:12)
2020-09-19T18:22:26.767114+00:00 app[web.1]: at Server.listen (net.js:1447:7)
2020-09-19T18:22:26.767115+00:00 app[web.1]: at Function.listen (/app/node_modules/express/lib/application.js:618:24)
2020-09-19T18:22:26.767115+00:00 app[web.1]: at Object.<anonymous> (/app/server.js:30:5)
2020-09-19T18:22:26.767115+00:00 app[web.1]: at Module._compile (internal/modules/cjs/loader.js:1137:30)
2020-09-19T18:22:26.767116+00:00 app[web.1]: at Object.Module._extensions..js (internal/modules/cjs/loader.js:1157:10)
2020-09-19T18:22:26.767116+00:00 app[web.1]: at Module.load (internal/modules/cjs/loader.js:985:32)
2020-09-19T18:22:26.767116+00:00 app[web.1]: at Function.Module._load (internal/modules/cjs/loader.js:878:14)
2020-09-19T18:22:26.767118+00:00 app[web.1]: at Function.executeUserEntryPoint [as runMain] (internal/modules/run_main.js:71:12)
2020-09-19T18:22:26.767118+00:00 app[web.1]: at internal/main/run_main_module.js:17:47
2020-09-19T18:22:26.767119+00:00 app[web.1]: Emitted 'error' event on Server instance at:
2020-09-19T18:22:26.767119+00:00 app[web.1]: at emitErrorNT (net.js:1340:8)
2020-09-19T18:22:26.767119+00:00 app[web.1]: at processTicksAndRejections (internal/process/task_queues.js:84:21) {
2020-09-19T18:22:26.767120+00:00 app[web.1]: code: 'EACCES',
2020-09-19T18:22:26.767121+00:00 app[web.1]: errno: 'EACCES',
2020-09-19T18:22:26.767121+00:00 app[web.1]: syscall: 'listen',
2020-09-19T18:22:26.767121+00:00 app[web.1]: address: '0.0.0.0',
2020-09-19T18:22:26.767122+00:00 app[web.1]: port: 1000
2020-09-19T18:22:26.767122+00:00 app[web.1]: }
2020-09-19T18:22:26.781861+00:00 app[web.1]: npm ERR! code ELIFECYCLE
2020-09-19T18:22:26.782206+00:00 app[web.1]: npm ERR! errno 1
2020-09-19T18:22:26.785690+00:00 app[web.1]: npm ERR! budget-app@1.0.0 start: `node server.js`
2020-09-19T18:22:26.786058+00:00 app[web.1]: npm ERR! Exit status 1
2020-09-19T18:22:26.786296+00:00 app[web.1]: npm ERR!
2020-09-19T18:22:26.786477+00:00 app[web.1]: npm ERR! Failed at the budget-app@1.0.0 start script.
2020-09-19T18:22:26.786638+00:00 app[web.1]: npm ERR! This is probably not a problem with npm. There is likely additional logging output above.
2020-09-19T18:22:26.796824+00:00 app[web.1]:
2020-09-19T18:22:26.797105+00:00 app[web.1]: npm ERR! A complete log of this run can be found in:
2020-09-19T18:22:26.797275+00:00 app[web.1]: npm ERR!     /app/.npm/_logs/2020-09-19T18_22_26_788Z-debug.log
2020-09-19T18:22:26.876075+00:00 heroku[web.1]: Process exited with status 1
2020-09-19T18:22:26.918227+00:00 heroku[web.1]: State changed from starting to crashed
2020-09-19T18:22:26.920187+00:00 heroku[web.1]: State changed from crashed to starting
2020-09-19T18:22:31.268167+00:00 heroku[web.1]: Starting process with command `npm start`
2020-09-19T18:22:34.783486+00:00 app[web.1]:
2020-09-19T18:22:34.783521+00:00 app[web.1]: > budget-app@1.0.0 start /app
2020-09-19T18:22:34.783522+00:00 app[web.1]: > node server.js
2020-09-19T18:22:34.783522+00:00 app[web.1]:
2020-09-19T18:22:35.645238+00:00 app[web.1]: events.js:292
2020-09-19T18:22:35.645281+00:00 app[web.1]: throw er; // Unhandled 'error' event
2020-09-19T18:22:35.645282+00:00 app[web.1]: ^
2020-09-19T18:22:35.645282+00:00 app[web.1]:
2020-09-19T18:22:35.645283+00:00 app[web.1]: Error: listen EACCES: permission denied 0.0.0.0:1000
2020-09-19T18:22:35.645284+00:00 app[web.1]: at Server.setupListenHandle [as _listen2] (net.js:1296:21)
2020-09-19T18:22:35.645284+00:00 app[web.1]: at listenInCluster (net.js:1361:12)
2020-09-19T18:22:35.645284+00:00 app[web.1]: at Server.listen (net.js:1447:7)
2020-09-19T18:22:35.645285+00:00 app[web.1]: at Function.listen (/app/node_modules/express/lib/application.js:618:24)
2020-09-19T18:22:35.645285+00:00 app[web.1]: at Object.<anonymous> (/app/server.js:30:5)
2020-09-19T18:22:35.645286+00:00 app[web.1]: at Module._compile (internal/modules/cjs/loader.js:1137:30)
2020-09-19T18:22:35.645286+00:00 app[web.1]: at Object.Module._extensions..js (internal/modules/cjs/loader.js:1157:10)
2020-09-19T18:22:35.645286+00:00 app[web.1]: at Module.load (internal/modules/cjs/loader.js:985:32)
2020-09-19T18:22:35.645287+00:00 app[web.1]: at Function.Module._load (internal/modules/cjs/loader.js:878:14)
2020-09-19T18:22:35.645287+00:00 app[web.1]: at Function.executeUserEntryPoint [as runMain] (internal/modules/run_main.js:71:12)
2020-09-19T18:22:35.645288+00:00 app[web.1]: at internal/main/run_main_module.js:17:47
2020-09-19T18:22:35.645288+00:00 app[web.1]: Emitted 'error' event on Server instance at:
2020-09-19T18:22:35.645288+00:00 app[web.1]: at emitErrorNT (net.js:1340:8)
2020-09-19T18:22:35.645289+00:00 app[web.1]: at processTicksAndRejections (internal/process/task_queues.js:84:21) {
2020-09-19T18:22:35.645289+00:00 app[web.1]: code: 'EACCES',
2020-09-19T18:22:35.645290+00:00 app[web.1]: errno: 'EACCES',
2020-09-19T18:22:35.645290+00:00 app[web.1]: syscall: 'listen',
2020-09-19T18:22:35.645290+00:00 app[web.1]: address: '0.0.0.0',
2020-09-19T18:22:35.645290+00:00 app[web.1]: port: 1000
2020-09-19T18:22:35.645291+00:00 app[web.1]: }
2020-09-19T18:22:35.664089+00:00 app[web.1]: npm ERR! code ELIFECYCLE
2020-09-19T18:22:35.664539+00:00 app[web.1]: npm ERR! errno 1
2020-09-19T18:22:35.668470+00:00 app[web.1]: npm ERR! budget-app@1.0.0 start: `node server.js`
2020-09-19T18:22:35.668694+00:00 app[web.1]: npm ERR! Exit status 1
2020-09-19T18:22:35.668978+00:00 app[web.1]: npm ERR!
2020-09-19T18:22:35.669198+00:00 app[web.1]: npm ERR! Failed at the budget-app@1.0.0 start script.
2020-09-19T18:22:35.669430+00:00 app[web.1]: npm ERR! This is probably not a problem with npm. There is likely additional logging output above.
2020-09-19T18:22:35.681584+00:00 app[web.1]:
2020-09-19T18:22:35.681882+00:00 app[web.1]: npm ERR! A complete log of this run can be found in:
2020-09-19T18:22:35.682073+00:00 app[web.1]: npm ERR!     /app/.npm/_logs/2020-09-19T18_22_35_671Z-debug.log
2020-09-19T18:22:35.760466+00:00 heroku[web.1]: Process exited with status 1
2020-09-19T18:22:35.807927+00:00 heroku[web.1]: State changed from starting to crashed
2020-09-19T18:22:41.260940+00:00 heroku[router]: at=error code=H10 desc="App crashed" method=GET path="/" host=mysterious-springs-16260.herokuapp.com request_id=999d8272-a83e-46f2-ba10-926bc76bdfa7 fwd="73.109.96.9" dyno= con
nect= service= status=503 bytes= protocol=https
2020-09-19T18:22:41.932541+00:00 heroku[router]: at=error code=H10 desc="App crashed" method=GET path="/favicon.ico" host=mysterious-springs-16260.herokuapp.com request_id=2db053be-36cf-43a1-9149-a8fd1fa8d072 fwd="73.109.96.9
" dyno= connect= service= status=503 bytes= protocol=https
2020-09-19T18:34:28.256237+00:00 heroku[router]: at=error code=H10 desc="App crashed" method=GET path="/" host=mysterious-springs-16260.herokuapp.com request_id=b011472c-f4ff-45cb-b100-f5c567ed9f8c fwd="73.109.96.9" dyno= con
nect= service= status=503 bytes= protocol=https
2020-09-19T18:34:28.659914+00:00 heroku[router]: at=error code=H10 desc="App crashed" method=GET path="/favicon.ico" host=mysterious-springs-16260.herokuapp.com request_id=f89efe9e-e25a-471a-8fb5-98af0cf6ba21 fwd="73.109.96.9
" dyno= connect= service= status=503 bytes= protocol=https
