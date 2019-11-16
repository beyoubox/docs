.. _query_stoken:

How to query Stoken data
==========================

|logo_etherscan_verified| |logo_github| |logo_verified|

- Contract address is **0x37C7e57f28f1c481Ffa354f5B21F159f8c51782b**
- Deployed at `Tx Hash 0xd88541481a39c1...`_
- Block height `#6495749`_
- Open-sourced under the `GNU General Public License v3.0`_
- `View contract code on github repository`_
- `View contract on Etherscan.io`_

.. _Tx Hash 0xd88541481a39c1...:
   https://etherscan.io/tx/0xd88541481a39c1e3b26e7cc93679d10466871c01675eae7f72892e16da0442fc
.. _#6495749:
   https://etherscan.io/block/6495749
.. _GNU General Public License v3.0:
   https://github.com/stoken100g/contracts/blob/master/LICENSE
.. _View contract code on github repository:
   https://github.com/stoken100g/contracts/blob/master/Stoken2Panel.sol
.. _View contract on Etherscan.io:
   https://etherscan.io/address/0x37C7e57f28f1c481Ffa354f5B21F159f8c51782b#readContract

.. |logo_github| image:: /_static/logos/github.svg
   :width: 36px
   :height: 36px

.. |logo_etherscan_verified| image:: /_static/logos/etherscan_verified.svg
   :width: 36px
   :height: 36px

.. |logo_verified| image:: /_static/logos/verified.svg
   :width: 36px
   :height: 36px


Here is the link for **Read the Contract**:
``https://etherscan.io/address/0x37C7e57f28f1c481Ffa354f5B21F159f8c51782b#readContract``

Click `here`_, then **Contract** => **Read Contract**

.. _here: https://etherscan.io/address/0x37C7e57f28f1c481Ffa354f5B21F159f8c51782b#readContract


Stoken summary
----------------

Function #2: **stoken2**

.. image:: /_static/contract/stoken2_summary.png
   :width: 80 %
   :align: center
   :alt: stoken2_summary.png

.. NOTE::

   totalSupply
      Total supply of Stoken, with 6 decimals.

      ``1000000000`` means **1,000,000,000.000 Stoken** total.


   whitelistCounter
      The counter for whitelisted addresses, with no decimals.

      ``6918`` means there are 6,918 addresses are already whitelisted.


   whitelistingMode
      Whether the whitelist signing-up is allowed.

      ``True`` for **YES**, and ``False`` for **NO**.

      When it shows ``True`` you can follow :ref:`how_to_join_the_whitelist` to join.


   safeMode
      Whether the **SAFE-MODE** is on.

      ``True`` for **YES**, and ``False`` for **NO**.

      When it shows ``True``, transfers from a non-whitelisted address is restricted.
      This is a mechanism to protect early ecological health.


   burningMode
      Whether the **BURNING-MODE** is on.

      ``True`` for **YES**, and ``False`` for **NO**.

      When it shows ``True``, **1%** will be **burned** for every transaction of Stoken.


   burningPermill
      When **BURNING-MODE** is on, the value is valid.
      It is the burning ratio in per-mill.

      ``10`` means the current burning ratio is **1%**.


Query an address in Stoken
----------------------------

Function #1: **queryAccount**

.. image:: /_static/contract/stoken2_query1.png
   :width: 80 %
   :align: center
   :alt: stoken2_query1.png

Enter an ETH wallet address, and press **Query**, then:

.. image:: /_static/contract/stoken2_query2.png
   :width: 80 %
   :align: center
   :alt: stoken2_query2.png


Let's focus on the returned values:

.. code-block:: text

   whitelisted               bool :     true
   whitelistReferralsCount   uint256 :  25
   balance                   uint256 :  118448326
   reserved                  uint256 :  59224163


.. NOTE::

   whitelisted
       If it returns ``true``, means the address is already whitelisted, ``false`` means no.


   whitelistReferralsCount
      The quantity of direct referrals.


   balance
      Balance of Stoken, with 6 decimals.
      ``118448326`` means **118.448326 Stoken**.


   reserved
      Reserved balance of Stoken, with 6 decimals.
      ``59224163`` means **59.224163 Stoken**.
