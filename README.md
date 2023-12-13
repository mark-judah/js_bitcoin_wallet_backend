<!DOCTYPE html>
<html>

<body>

<h1>Bitcoin Core Testnet Setup</h1>

<h2>Installing Bitcoin Core Testnet</h2>

<p>To set up Bitcoin Core running a full testnet node:</p>
<ol>
  <li>Download and install Bitcoin Core from the official website.</li>
  <li>Run Bitcoin Core with the following command to set up for testnet:</li>
  <pre><code>
  bitcoind -testnet -daemon
  </code></pre>
  <li>Wait for the blockchain to sync (this may take some time).</li>
</ol>

<h2>Node.js Backend Project Setup</h2>

<h3>Setting Up the Node.js Backend</h3>
<p>The Node.js backend links to the locally installed Bitcoin Core testnet and exposes the following API routes:</p>

<ul>
  <li>/createMnemonic</li>
  <li>/createWalletSeed</li>
  <li>/createWallet</li>
  <li>/setWalletSeed</li>
  <li>/getWalletInfo</li>
  <li>/loadWallet</li>
  <li>/getNewAddress</li>
  <li>/deriveReceivingAddress</li>
  <li>/getAddressInfo</li>
  <li>/getReceivedByAddress</li>
  <li>/listTransactions</li>
  <li>/listUnspentTransactions</li>
  <li>/createRawTransaction</li>
  <li>/signRawTransaction</li>
  <li>/dumpWallet</li>
  <li>/sendRawTransaction</li>
  <li>/getBalances</li>
  <li>/getTransaction</li>
  <li>/unloadWallet</li>
  <li>/dumpPrivKey</li>
  <li>/deriveChangeAddress</li>
  <li>/loadWalletRequest</li>
</ul>

<h3>Backend Setup Instructions</h3>
<ol>
  <li>Clone the Node.js backend repository.</li>
  <pre><code>
  git clone https://github.com/your-username/your-nodejs-backend.git
  </code></pre>
  <li>Install project dependencies:</li>
  <pre><code>
  cd your-nodejs-backend
  npm install
  </code></pre>
  <li>Set up environment variables for connecting to the Bitcoin Core testnet.</li>
  <li>Run the Node.js backend:</li>
  <pre><code>
  npm start
  </code></pre>
</ol>

<h2>API Usage</h2>
<p>The mobile client can make requests to the Node.js backend API routes to interact with the Bitcoin Core testnet as needed.</p>


</body>
</html>