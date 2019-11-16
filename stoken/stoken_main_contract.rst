.. _stoken2_main_contract:

Stoken Main Contract
=======================

This is the **MAIN CONTRACT** of :ref:`stoken`, updated and deployed at ``2019-10-02 16:12:41 UTC``.

|logo_etherscan_verified| |logo_github| |logo_verified|

- Contract address is **0x37C7e57f28f1c481Ffa354f5B21F159f8c51782b**
- Deployed at `Tx Hash 0xd88541481a39c1e3b26e7cc93679d10466871c01675eae7f72892e16da0442fc`_
- Block height `#6495749`_
- Open-sourced under the `GNU General Public License v3.0`_
- `View contract code on github repository`_

View on Etherscan.io:

- `Stoken transactions tracker`_
- `View transactions and interactions of the contract`_
- `Read contract on Etherscan.io`_
- `Write contract on Etherscan.io`_

.. _Tx Hash 0xd88541481a39c1e3b26e7cc93679d10466871c01675eae7f72892e16da0442fc:
   https://etherscan.io/tx/0xd88541481a39c1e3b26e7cc93679d10466871c01675eae7f72892e16da0442fc
.. _#6495749:
   https://etherscan.io/block/6495749
.. _GNU General Public License v3.0:
   https://github.com/beyoubox/contracts/LICENSE
.. _View contract code on github repository:
   https://github.com/beyoubox/contracts/BeyouCoin.sol
.. _Stoken transactions tracker:
   https://etherscan.io/token/0x37C7e57f28f1c481Ffa354f5B21F159f8c51782b
.. _View transactions and interactions of the contract:
   https://etherscan.io/address/0x37C7e57f28f1c481Ffa354f5B21F159f8c51782b
.. _Read contract on Etherscan.io:
   https://etherscan.io/address/0x37C7e57f28f1c481Ffa354f5B21F159f8c51782b#readContract
.. _Write contract on Etherscan.io:
   https://etherscan.io/address/0x37C7e57f28f1c481Ffa354f5B21F159f8c51782b#writeContract


.. |logo_github| image:: /_static/logos/github.svg
   :width: 36px
   :height: 36px

.. |logo_etherscan_verified| image:: /_static/logos/etherscan_verified.svg
   :width: 36px
   :height: 36px

.. |logo_verified| image:: /_static/logos/verified.svg
   :width: 36px
   :height: 36px


The token symbol named ``Stoken``
-----------------------------------

Displayed in various wallet software such as `MetaMask`_,
`MyEtherWallet`_, `imToken`_, `etherscan.io`_ and Ethereum blockchain browsers.

.. _MetaMask: https://metamask.io/
.. _MyEtherWallet: https://www.myetherwallet.com/
.. _imToken: https://imkey.im/
.. _etherscan.io: https://etherscan.io/


Features and functions
----------------------

.. _stoken_based_on_erc20:

Based on `[EIP 20] ERC-20 Token Standard`_ of `Ethereum`_
   Includes:

   - ``function name() public view returns (string)``
   - ``function symbol() public view returns (string)``
   - ``function decimals() public view returns (uint8)``
   - ``function totalSupply() public view returns (uint256)``
   - ``function balanceOf(address account) public view returns (uint256)``
   - ``function transfer(address recipient, uint256 amount) public returns (bool)``
   - ``function transferFrom(address sender, address recipient, uint256 amount) public returns (bool)``
   - ``function approve(address spender, uint256 value) public returns (bool)``
   - ``function allowance(address owner, address spender) public view returns (uint256)``
   - ``event Transfer(address indexed from, address indexed to, uint256 value)``
   - ``event Approval(address indexed owner, address indexed spender, uint256 value)``

   With advanced functions for allowance:

   - ``function increaseSupply(address spender, uint256 addedValue) public returns (bool)``
   - ``function decreaseSupply(address spender, uint256 subtractedValue) public returns (bool)``


.. _[EIP 20] ERC-20 Token Standard: https://eips.ethereum.org/EIPS/eip-20
.. _Ethereum: https://www.ethereum.org


.. _stoken_supports_freezing:

Supports flexible rules for **LOCK**
   Function for lock:

   - ``function lock(address _addr, uint256 _value) external returns (uint256)``

   Function for unlock:

   - ``function unlock(address _addr, uint256 _value) public returns (uint256)``
