Open 2 terminals and execute
$ reach run

Just select the appropiate option on console

Choose and one participant in each one (Alice, Bob)

By developemt purpose select create an account option

Alice shall be participant who creates the contract.
Annotate the contract number and pass to Bob 

select the wage, the hand and enjoy :)

............................................
Output sample execution:
Alice:
sese@SUPERPEPINILLO:~/reach/tut/reach_lang/RockPaperScissors/Console$ reach run
[+] Building 0.2s (7/7) FINISHED
 => [internal] load build definition from Dockerfile                                                                                 0.0s
 => => transferring dockerfile: 235B                                                                                                 0.0s
 => [internal] load .dockerignore                                                                                                    0.0s
 => => transferring context: 75B                                                                                                     0.0s
 => [internal] load metadata for docker.io/reachsh/runner:0.1.7                                                                      0.0s
 => [internal] load build context                                                                                                    0.0s
 => => transferring context: 1.08kB                                                                                                  0.0s
 => CACHED [1/2] FROM docker.io/reachsh/runner:0.1.7                                                                                 0.0s
 => [2/2] COPY . /app                                                                                                                0.1s
 => exporting to image                                                                                                               0.1s
 => => exporting layers                                                                                                              0.0s
 => => writing image sha256:4f24f2c833f9b8e3e10a6d22231913747f337195f2a667a5f3ddf159fee77dec                                         0.0s
 => => naming to docker.io/reachsh/reach-app-console:0.1.7                                                                           0.0s

Use 'docker scan' to run Snyk tests against images to find vulnerabilities and learn how to fix them

> @reach-sh/console@ index /app
> node --experimental-modules --unhandled-rejections=strict index.mjs

Are you Alice?
y
Starting Rock, Paper, Scissors! as Alice
Would you like to create an account? (only possible on devnet)
y
Your balance is 1000
How much do you want to wager?
100
The contract is deployed as = 352
What hand will you play?
p
You played Paper
The outcome is: Bob wins
Your balance is now 899.9929

Bob:
sese@SUPERPEPINILLO:~/reach/tut/reach_lang/RockPaperScissors/Console$ reach run
[+] Building 0.1s (7/7) FINISHED
 => [internal] load build definition from Dockerfile                                                                                 0.0s
 => => transferring dockerfile: 38B                                                                                                  0.0s
 => [internal] load .dockerignore                                                                                                    0.0s
 => => transferring context: 34B                                                                                                     0.0s
 => [internal] load metadata for docker.io/reachsh/runner:0.1.7                                                                      0.0s
 => [internal] load build context                                                                                                    0.0s
 => => transferring context: 356B                                                                                                    0.0s
 => [1/2] FROM docker.io/reachsh/runner:0.1.7                                                                                        0.0s
 => CACHED [2/2] COPY . /app                                                                                                         0.0s
 => exporting to image                                                                                                               0.1s
 => => exporting layers                                                                                                              0.0s
 => => writing image sha256:4f24f2c833f9b8e3e10a6d22231913747f337195f2a667a5f3ddf159fee77dec                                         0.0s
 => => naming to docker.io/reachsh/reach-app-console:0.1.7                                                                           0.0s

Use 'docker scan' to run Snyk tests against images to find vulnerabilities and learn how to fix them

> @reach-sh/console@ index /app
> node --experimental-modules --unhandled-rejections=strict index.mjs

Are you Alice?
n
Starting Rock, Paper, Scissors! as Bob
Would you like to create an account? (only possible on devnet)
y
Please paste the contract information:
352
Your balance is 1000
Do you accept the wager of 100?
y
What hand will you play?
s
You played Scissors
The outcome is: Bob wins
Your balance is now 1099.997
