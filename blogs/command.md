cat /proc/meminfo
 firewall-cmd --list-all
 view /etc/sysconfig/networkせとぎわかみひとえ


php artisan make:migration create_master_card_table --create=master_card
php artisan make:seeder UserSeeder

php artisan make:controller PurchaseController --resource --model=Purchase

geth --rinkeby --syncmode=fast --cache=2048
geth --rinkeby account new
geth --rinkeby --verbosity 0 console

eth.sendTransaction({
from: eth.accounts[0],
to: "0x07afc8F81Fdd6eF02C116cccF116cFD5864800aC", value: 1e17,
gas: 90e3,
gasPrice: 20e9
})
personal.unlockAccount(eth.accounts[0], password)

remixd -s /Users/ace/work/game_blockchain/source/nifty-game  --remix-ide https://remix.ethereum.org

begin nifty-game
ganache-cli --gasLimit 0xffffffffff -p 8545
geth attach http://127.0.0.1:8545
curl -X POST --data '{"jsonrpc":"2.0","method":"eth_sendTransaction","params":[{"from": "0xdd940cc5fefb7e32bd8d5307f674ed9b6d27c092", "to": "0x1b7543ECeA2ccbEFfCc3231117350Af4B818428B", value: "10000000000000000", data: "0x1249c58b"}],"id":1}' http://localhost:8545


curl -X POST --data '{"id":5976625957778,"jsonrpc":"2.0","params":["0xf8721b850430e23400836170d4941b7543ecea2ccbeffcc3231117350af4b818428b872386f26fc10000841249c58b822d45a057daba1214011be74537cd3e7c3f789b200642eddf19963ba3f554ea69fd3e8ea02a74e67634ff85bce9f4f71a706dd4b7649d2d066d3f4e6374419226e1f48fcc"],"method":"eth_sendRawTransaction"' http://localhost:8545



curl -X POST --data '{"jsonrpc":"2.0","method":"eth_sendTransaction","params":[{"from": "0xd4f94003d484b2152Ba500418c5FDdaaa6ccfB6F", "to": "0x1b7543ECeA2ccbEFfCc3231117350Af4B818428B", value: "10000000000000000", data: "0x1249c58b"}],"id":1}' http://localhost:8545


sudo npm install -g --unsafe-perm=true --allow-root

METoken.deployed().then(instance => { instance.balanceOf(accounts[0]).then(console.log) })

METoken.deployed().then(instance => { instance.transfer(accounts[2], 100000) })


METoken.deployed().then(instance => { instance.balanceOf(accounts[2]).then(console.log) })


METoken.deployed().then(instance => { instance.transfer(Faucet.address, 100000) })


METoken.deployed().then(instance => { instance.balanceOf(Faucet.address).then(console.log)})

 METoken.deployed().then(instance => { instance.balanceOf(Faucet.address).then(a => console.log(a.toNumber()))})


METoken.deployed().then(instance => { instance.approve(METFaucet.address, 100000) })



METoken.deployed().then(instance => { instance.balanceOf(web3.eth.accounts[2]).then(console.log) })

METFaucet.deployed().then(instance => { instance.withdraw(1000, {from:accounts[1]}) } )
