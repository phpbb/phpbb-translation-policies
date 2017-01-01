# Language Pack Submission Policy

Below are the procedures and guidelines that need to be followed by any translator submitting a language pack to our Customisation Database.
All approved language packs can be found in our [Language Packs Database](https://www.phpbb.com/languages/ "Language Packs Database").
If you submit your language pack to our Customisation Database, it will first be automatically sent to the Translations Manager for validation.
He is responsible for ensuring that your submission follows the guidelines below.
Failure to comply with the following instructions could lead to an instant denial of your submission.
Please note the Translations Manager has full discretion on what he approves or denies.
This process can sometimes take a considerable amount of time, so it's in your best interest to follow all of the guidelines from the start.
If your language pack is denied and then resubmitted, it is placed at the end of the queue.

1. Submissions have to be compatible with the latest version of phpBB. Any missing key will be detected during the upload process and your submission will be automatically denied.


2. Submissions have to be complete. Partial translations are not allowed and will be systematically denied. E-mail text files and theme-images must also be fully translated. Only `search_ignore_words.php` and `search_synonyms.php` are allowed to be untranslated. However, they must still be included, have the basic file structure and just an empty array `$words` or `$synonyms` respectively.


3. Language packs can contain five additional files (one mandatory and four optionals) that are not present in the British English language pack: `LICENSE` (mandatory), `README` / `README.md` (optional), `AUTHORS` / `AUTHORS.md` (optional), `VERSION` / `VERSION.md` (optional) and `CHANGELOG` / `CHANGELOG.md` (optional). 
You are free to write whatever you want in the `README` file, you can list all the authors and contributors of your language pack in the `AUTHORS` file, you can put the version of your language pack in the `VERSION` file and you can list all the version history in the `CHANGELOG` file.
Concerning the `LICENSE` file, it is automatically added during the upload process, you do not have to manually add it. It tells to the user the license used.
Language packs inherits phpBB's license [GNU General Public License 2.0](http://www.opensource.org/licenses/gpl-2.0.php "GNU General Public License 2.0"), and no additional or alternative licenses are allowed.
These files must be placed in the `language/{iso}/` directory, next to the `iso.txt` file. Any other additional file will be detected and your submission will be denied.


4. Submissions must have the following files and structure:

        languagename_versionnumber.zip
           languagename_versionnumber/
              ext/
                 phpbb/
                    viglink/
                       language/
                          {iso}/
                             info_acp_viglink.php
                             viglink_module_acp.php
              language/
                 {iso}/
                    acp/
                       attachments.php
                       ban.php
                       board.php
                       bots.php
                       common.php
                       database.php
                       email.php
                       extensions.php
                       forums.php
                       groups.php
                       index.htm (optional)
                       language.php
                       modules.php
                       permissions.php
                       permissions_phpbb.php
                       posting.php
                       profile.php
                       prune.php
                       search.php
                       styles.php
                       users.php
                    email/
                       short/
                          bookmark.txt
                          index.htm (optional)
                          newtopic_notify.txt
                          post_approved.txt
                          post_disapproved.txt
                          post_in_queue.txt
                          privmsg_notify.txt
                          quote.txt
                          report_pm.txt
                          report_post.txt
                          topic_approved.txt
                          topic_disapproved.txt
                          topic_in_queue.txt
                          topic_notify.txt
                       admin_activate.txt
                       admin_send_email.txt
                       admin_welcome_activated.txt
                       admin_welcome_inactive.txt
                       bookmark.txt
                       contact_admin.txt
                       coppa_resend_inactive.txt
                       coppa_welcome_inactive.txt
                       email_notify.txt
                       forum_notify.txt
                       group_added.txt
                       group_request.txt
                       index.htm (optional)
                       installed.txt
                       newtopic_notify.txt
                       pm_report_closed.txt
                       pm_report_deleted.txt
                       post_approved.txt
                       post_disapproved.txt
                       post_in_queue.txt
                       privmsg_notify.txt
                       profile_send_email.txt
                       profile_send_im.txt
                       quote.txt
                       report_closed.txt
                       report_deleted.txt
                       report_pm.txt
                       report_post.txt
                       test.txt
                       topic_approved.txt
                       topic_disapproved.txt
                       topic_in_queue.txt
                       topic_notify.txt
                       user_activate.txt
                       user_activate_inactive.txt
                       user_activate_passwd.txt
                       user_reactivate_account.txt
                       user_remind_inactive.txt
                       user_resend_inactive.txt
                       user_welcome.txt
                       user_welcome_inactive.txt
                    help/
                       bbcode.php
                       faq.php
                    app.php
                    AUTHORS (optional)
                    captcha_qa.php
                    captcha_recaptcha.php
                    cli.php
                    CHANGELOG (optional)
                    common.php
                    groups.php
                    index.htm (optional)
                    install.php
                    iso.txt
                    LICENSE
                    mcp.php
                    memberlist.php
                    migrator.php
                    plupload.php
                    posting.php
                    README (optional)
                    search.php
                    ucp.php
                    VERSION (optional)
                    viewforum.php
                    viewtopic.php
              styles/
                 prosilver/
                    theme/
                       {iso}/
                          icon_user_online.gif
                          index.htm (optional)
                          stylesheet.css

5. Submissions have to follow as much as possible the [3.2 Translation (i18n/L10n) Guidelines](https://area51.phpbb.com/docs/32x/coding-guidelines.html#translation "3.2 Translation (i18n/L10n) Guidelines") recommandantions, especially the [3.2 Writing style](https://area51.phpbb.com/docs/32x/coding-guidelines.html#writingstyle "3.2 Writing style").


6. All the PHP and text files have to be encoding in UTF-8 without BOM and a new line at the end of the file. Many modern text editors use this as a default setting, but we recommend checking it in your editor's settings.
We recommend you [Notepad++](https://notepad-plus-plus.org/ "Notepad++") or [PSPad](http://www.pspad.com/en/ "PSPad"), both lightweight and free.


7. The translation is mostly your work and you have a right to hold a copyright and names to it.


8. A maximum of 3 links can be included as an author credit in the footer, customisable via the `'TRANSLATION_INFO'` key in `common.php`.
Please note that the Translations Manager has complete discretion on what is acceptable as an author credit link.


9. Submissions have to be submitted as a single zip file. For information, the Customisation Database will automatically name `languagename_versionnumber.zip` your uploaded language pack.
For example, if a Brazilian Portuguese language pack author uploads an archive named `Brasileiro_1.0.5.zip`, it will be automatically changed to `brazilian_portuguese_1_0_5.zip`.


10. Contribution description in the Customisation Database should be translated into English in addition of your local language.
Some administrators might want to download your translation without speak your language.


11. Contribution screenshot in the Customisation Database should only be the flag of the country whose the language is spoken.
For example, the flag of France for the French language.


12. Revision name in the Customisation Database should be left blank, contain the phpBB package version and/or package release name (e.g. "**3.0.12 / Richard 'D¡cky' Foote**" for 3.0.12) for more understanding.


13. The Demo URL in the Customisation Database must be empty, unless you want to put a link to an international community ([officially](https://www.phpbb.com/support/intl/ "officially") listed or not) related to the language of the contribution.
For example, http://www.phpbbarabia.com/ as Demo URL concerning the [Arabic language](https://www.phpbb.com/customise/db/translation/arabic/ "Arabic language") is allowed.
