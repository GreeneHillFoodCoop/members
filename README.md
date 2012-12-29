members
=======
This has the CiviCRM and Drupal files for the coop's member website.

How to push changes
-------------------
1. Clone the repo, edit a file, commit, and push back to Github:
        $ git clone git@github.com:GreeneHillFoodCoop/members.git
        $ cd members/
        ... edit file sites/all/modules/civicrm/css/civicrm.css
        $ git status
        $ git commit -a -m"Sample change to civicrm.css"
        $ git push

2. Now pull from GitHub into the server dir:
        $ ssh deploy@kale.greenehillfood.coop members-staging
        From git://github.com/GreeneHillFoodCoop/members
         * branch            master     -> FETCH_HEAD
        Updating e6c03d5..3ae0247
        Fast-forward
         .gitignore                                |    1 +
         sites/all/modules/civicrm/css/civicrm.css |    2 +-
         2 files changed, 2 insertions(+), 1 deletion(-)

That's it!
