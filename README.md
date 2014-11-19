# The Binding of Isaac Rebirth for the Death Roulette

You can use this repository as a base to set up more games for the Death Roulette.

Edit the ``manifest.json`` file to match the game you want to support:

 * It must contain ``title``, ``hostBetId`` and ``groups`` keys.
 * You can add or remove groups (like ``Hazards`` and ``Places``), they are not fixed.
 * In each group:
   * ``bets`` must be a number that limits the number of different bets one can place on that group
   * ``size`` must contain a ``width`` and ``height`` for all the bet images for this group
   * ``categories`` should contain lists of bet option by categories (you decide how to categorize them)
   * Alternatively, you can replace ``categories`` with ``all`` if you have no sub-categories (see [Crypt of the Necrodancer for an example](https://bitbucket.org/sparklinlabs/deathroulette-necrodancer/src/tip/manifest.json?at=default#cl-49))

Then place all the bet images in the ``groups`` folder, zip it all up and [email it to Elisee](mailto:elisee@sparklinlabs.com). He'll review it and add it to the roster of games.