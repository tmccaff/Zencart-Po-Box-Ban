Name
====
PO Box Ban

Version 1.6 tested on 1.5.6c; updated by tmccaff
For this version it should be ok to just upload to your server.
What I was told is that you don't need to add this to your shipping module like before.
Tested it and seems to work. This mod does change the core, so backup before installing.

any issues go to support thread listed below.

Version Date
============
1.6 08/11/2019
1.5 1/18/2018 
1.4 10.03.2012

Author
======
mvstudio

Description
===========
We were facing the problem of having clients with PO boxes as
shipping before we installed the 1.3 version of this module. So we made
some changes to make this module work for our store even if PO box
addresses were already in the database.

This new version allows a customer to change their billing address to
a PO box, but doesn't allow them to change the shipping address to a PO Box. 
Also will display an error message on the checkout_shipping page if a 
PO box appears as a shipping address, assuming it was present in the
database before this module was installed.

This mod effectively bans PO Box addresses from being used on your store.

It works by comparing the customer's address at sign-up with a range of 
words/letters often used with these addresses. Errors are displayed via the
messageStack. The 'add shipping address' at checkout is also validated.

Installation is simple.

For support/feedback, https://www.zen-cart.com/showthread.php?99784-PO-Box-Ban-support-thread



Modified Files
-----
includes/modules/pages/address_book_process/header_php.php
includes/modules/checkout_new_address.php
includes/modules/create_account.php

New Files
-----
includes/languages/english/extra_definitions/po_box_ban_defines.php

Affects DB
==========
- none -


Installation
=======

0. BACKUP! BACKUP! BACKUP! BACKUP! BACKUP! BACKUP!

1. Upload the new files to the server in their respective folders


************************************************************


Uninstall
=========
Delete or unmerge the following files:
includes/languages/english/extra_definitions/po_box_ban_defines.php
includes/modules/create_account.php
includes/modules/checkout_new_address.php
includes/modules/pages/address_book_process/header_php.php





History
=======
1. Initial version 											1.0 		04.06.2008
2. Avoids core file change									1.0.1		05.06.2008
3. Validate 'My Account' option                				1.2		26.06.2008
4. Improves accuracy of detection							1.3		07.01.2009
5. Improves accuracy of detection, better functionality 	1.4		03.10.2012
6. Updated for Zencart 1.5.5f                 1.5             01.12.2018
7. Updated for Zencart 1.5.6c                 1.6             08.11.2019


DISCLAIMER
==========
This program is free software; you can redistribute it and/or
modify it under the terms of the GNU General Public License
as published by the Free Software Foundation; either version 2
of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
GNU General Public License for more details.

You should have received a copy of the GNU General Public License
(LICENSE) along with this program; if not, write to the Free Software
Foundation, Inc., 59 Temple Place - Suite 330, Boston, MA  02111-1307, USA.

Installation of this contribution is done at your own risk.
Backup your Zen Cart database and any and all applicable files before proceeding.
