<h2 dir="auto">Overview</h2>
<p dir="auto">The Seedx token repository is an exhaustive and up-to-date database of data on hundreds of different types of cryptocurrency tokens.</p>
<p dir="auto"><a href="https://seedx.app" rel="nofollow">Seedx</a> Like many other initiatives, draws its token logos from this collection.</p>
<p dir="auto">The token data repository stores data from several blockchains, including data on dApps, staking validators, etc. Each token may have its own unique logo and accompanying details (such data is not available on-chain).</p>
<p dir="auto">Such a large collection can be maintained only through a community effort, so <em>feel free to add your token</em>.</p>
<p dir="auto"><a href="https://camo.githubusercontent.com/9867493e3fbfe94363795eb74da50bcfe64e96220b0c862956d8b2aa7c5715b7/68747470733a2f2f747275737477616c6c65742e636f6d2f6173736574732f696d616765732f6d656469612f6173736574732f686f72697a6f6e74616c5f626c75652e706e67" rel="noopener noreferrer nofollow" target="_blank"><img src="https://camo.githubusercontent.com/9867493e3fbfe94363795eb74da50bcfe64e96220b0c862956d8b2aa7c5715b7/68747470733a2f2f747275737477616c6c65742e636f6d2f6173736574732f696d616765732f6d656469612f6173736574732f686f72697a6f6e74616c5f626c75652e706e67" height="200"></a></p>
<h2 dir="auto"><br></h2>
<h2 dir="auto">How to add token</h2>
<p dir="auto">Please note that <strong>brand new tokens are not accepted</strong>, the projects have to be sound, with information available, and <strong>non-minimal circulation</strong> (for limit details see <a href="https://developer.trustwallet.com/assets/requirements" rel="nofollow">https://developer.trustwallet.com/assets/requirements</a>).</p>
<h3 dir="auto"><br></h3>
<h3 dir="auto">Assets App</h3>
<p dir="auto">The <a href="https://assets.trustwallet.com" rel="nofollow">Assets web app</a> can be used for most new token additions (Github account is needed).</p>
<h3 dir="auto"><br></h3>
<h3 dir="auto">Quick starter</h3>
<p dir="auto">Details of the repository structure and contribution guidelines are listed on the <a href="https://developer.trustwallet.com/assets/new-asset" rel="nofollow">Developers site</a>. Here is a quick starter summary for the most common use case.</p>
<h2 dir="auto"><br></h2>
<h2 dir="auto">Documentation</h2>
<p dir="auto">For details, see the <a href="https://developer.trustwallet.com" rel="nofollow">Developers site</a>:</p>
<ul dir="auto">
    <li>
        <p dir="auto"><a href="https://developer.trustwallet.com/assets/repository_details" rel="nofollow">Contribution guidelines</a></p>
    </li>
    <li>
        <p dir="auto"><a href="https://developer.trustwallet.com/assets/faq" rel="nofollow">FAQ</a></p>
    </li>
</ul>
<h2 dir="auto"><br></h2>
<h2 dir="auto">Scripts</h2>
<p dir="auto">There are several scripts available for maintainers:</p>
<ul dir="auto">
    <li><code>make check</code> -- Execute validation checks; also used in continuous integration.</li>
    <li><code>make fix</code> -- Perform automatic fixes where possible</li>
    <li><code>make update-auto</code> -- Run automatic updates from external sources, executed regularly (GitHub action)</li>
    <li><code>make add-token asset_id=c60_t0x4Fabb145d64652a948d72533023f6E7A623C7C53</code> -- Create <code>info.json</code> file as asset template.</li>
    <li><code>make add-tokenlist asset_id=c60_t0x4Fabb145d64652a948d72533023f6E7A623C7C53</code> -- Adds a token to tokenlist.json.</li>
    <li><code>make add-tokenlist-extended asset_id=c60_t0x4Fabb145d64652a948d72533023f6E7A623C7C53</code> -- Adds a token to tokenlist-extended.json.</li>
</ul>
<h2 dir="auto"><br></h2>
<h2 dir="auto">On Checks</h2>
<p dir="auto">This repo contains a set of scripts for verification of all the information. Implemented as Golang scripts, available through <code>make check</code>, and executed in CI build; checks the whole repo. There are similar check logic implemented:</p>
<ul dir="auto">
    <li>in assets-management app; for checking changed token files in PRs, or when creating a PR. &nbsp;Checks diffs, can be run from browser environment.</li>
    <li>in merge-fee-bot, which runs as a GitHub app shows result in PR comment. Executes in a non-browser environment.</li>
</ul>
<h2 dir="auto"><br></h2>
<h2 dir="auto">Trading pair maintenance</h2>
<p dir="auto">Info on supported trading pairs are stored in <code>tokenlist.json</code> files. Trading pairs can be updated -- from Uniswap/Ethereum and PancakeSwap/Smartchain -- using update script (and checking in changes). Minimal limit values for trading pair inclusion are set in the <a href="https://github.com/trustwallet/assets/blob/master/.github/assets.config.yaml">config file</a>. There are also options for force-include and force-exclude in the config.</p>
<h2 dir="auto"><br></h2>
<h2 dir="auto">Disclaimer</h2>
<p dir="auto">Seedx team allows anyone to submit new assets to this repository. However, this does not mean that we are in direct partnership with all of the projects.</p>
<p dir="auto">Seedx team will reject projects that are deemed as scam or fraudulent after careful review. Trust Wallet team reserves the right to change the terms of asset submissions at any time due to changing market conditions, risk of fraud, or any other factors we deem relevant.</p>
<p dir="auto">Additionally, spam-like behavior, including but not limited to mass distribution of tokens to random addresses will result in the asset being flagged as spam and possible removal from the repository.</p>
