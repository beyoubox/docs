.. _how_to_join_the_whitelist:

How to join the whitelist
=========================

- Is there a friend told you about Beyou Network, :ref:`stoken`, and :ref:`stoken2_sale`?
  Congratulations!! Ask him for a **whitelisted address**.
- Use your ETH wallet, send **1,001 Stoken** to the address which is whitelisted already.
- You will receive **1 Stoken** back, as a success signal.
- Finished. Your wallet address has already whitelisted.


.. NOTE::

   Set ``gas limit`` to ``600,000`` or more,
   the rest will be returned automatically.

   Related link: :ref:`gas`


.. _FAQ_about_whitelist:

FAQ about whitelist
-------------------

How can I check whether a wallet address is whitelisted， and its referral count?
   | :ref:`query_stoken` on Etherscan.io:
   | ``https://etherscan.io/address/0x37C7e57f28f1c481Ffa354f5B21F159f8c51782b#readContract``
   |
   | **Contract** => **Read Contract**:

   Function #1: **queryAccount**

   .. image:: /_static/contract/stoken2_query1.png
      :width: 80 %
      :align: center
      :alt: stoken2_query1.png

   |

   Enter an ETH wallet address, and press **Query**, then:

   .. image:: /_static/contract/stoken2_query2.png
      :width: 80 %
      :align: center
      :alt: stoken2_query2.png

Where could I buy some Stoken?
   There may be these ways:

   - Participate in :ref:`stoken2_sale`, send ETH to buy.
   - Follow :ref:`get_1001stoken2`.
   - Ask your friend to send you some.


After my address was whitelisted, what will happen if I send 1,001.0 Stoken to my friend or others?
   Just like normal transfer,
   whitelist registration couldn't be trigger twice.
