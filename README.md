# hello-wolrd
@@ -1,38 +1,51 @@
-moneybitcoin - a lite version of Bitcoin optimized for CPU mining using scrypt as a proof of work scheme.
- - 2.5 minute block targets
- - subsidy halves in 840k blocks (~4 years)
- - ~84 million total coins
-
-The rest is the same as bitcoin.
- - 50 coins per block
- - 2016 blocks to retarget difficulty
-
-Development process
-===================
-
-Developers work in their own trees, then submit pull requests when
-they think their feature or bug fix is ready.
-
-The patch will be accepted if there is broad consensus that it is a
-good thing.  Developers should expect to rework and resubmit patches
-if they don't match the project's coding conventions (see coding.txt)
-or are controversial.
-
-The master branch is regularly built and tested, but is not guaranteed
-to be completely stable. Tags are regularly created to indicate new
-official, stable release versions of moneybitcoin.
-
-Feature branches are created when there are major new features being
-worked on by several people.
-
-From time to time a pull request will become outdated. If this occurs, and
-the pull is no longer automatically mergeable; a comment on the pull will
-be used to issue a warning of closure. The pull will be closed 15 days
-after the warning if action is not taken by the author. Pull requests closed
-in this manner will have their corresponding issue labeled 'stagnant'.
-
-Issues with no commits will be given a similar warning, and closed after
-15 days from their last activity. Issues closed in this manner will be 
-labeled 'stale'. 
-
-Check out http://forum.moneybitcoin.net/index.php/board,2.0.html for more info about the development.
+SmallChange (SMC) - a 'faster' version of moneybitcoin which also uses scrypt
+as a proof of work scheme and is intended for microtransactions.
+ - 15 seconds block targets: beat that MinCoin! ;)
+ - 420 699 680 total coins
+ - no subsidy within the first 3 days and after approximately 5 years;
+    in between: 4 coins per generated block
+ - difficulty retargets every 0.35 days
+ - currently peers are looked up over IRC only
+ - currently no block checkpoints are in the code (but could be easily
+   added)
+Other than that, this coin is exactly like moneybitcoin and should by no
+means be used as a real cryptocurrency. All of the coin parameters
+are chosen arbitrarily or at most with 'fairness' towards everyone in mind.
+
+So actually, this 'new' coin exists for the following reasons:
+ - SMC proves that really anyone(!) can start a moneybitcoin/Bitcoin based currency
+    (just look at the changes I applied to the original moneybitcoin source,
+     for genesis block generation look at main.cpp)
+ - allows me to experiment with coin parameters (in a private network)
+
+Finally, I only tested the command line server/tool 'smallchange' for the
+first 30 blocks. Credits go to the original authors/communities that
+created Bitcoin and moneybitcoin.
+
+Development process
+===================
+
+Developers work in their own trees, then submit pull requests when
+they think their feature or bug fix is ready.
+
+The patch will be accepted if there is broad consensus that it is a
+good thing.  Developers should expect to rework and resubmit patches
+if they don't match the project's coding conventions (see coding.txt)
+or are controversial.
+
+The master branch is regularly built and tested, but is not guaranteed
+to be completely stable. Tags are regularly created to indicate new
+official, stable release versions of moneybitcoin.
+
+Feature branches are created when there are major new features being
+worked on by several people.
+
+From time to time a pull request will become outdated. If this occurs, and
+the pull is no longer automatically mergeable; a comment on the pull will
+be used to issue a warning of closure. The pull will be closed 15 days
+after the warning if action is not taken by the author. Pull requests closed
+in this manner will have their corresponding issue labeled 'stagnant'.
+
+Issues with no commits will be given a similar warning, and closed after
+15 days from their last activity. Issues closed in this manner will be 
+labeled 'stale'.
