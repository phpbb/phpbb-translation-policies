# Language Packs Submission Policy

Below are the procedures and guidelines that need to be followed by any translator submitting a language pack to our Customisation Database. All approved language packs can be found in our [Language Packs Database](https://www.phpbb.com/customise/db/language_packs-25/ "Language Packs Database"). If you submit your language pack to our Customisation Database, it will first be automatically sent to the Translations & International Support Teams Manager for validation. He is responsible for ensuring that your submission follows the guidelines below. Failure to comply with the following instructions could lead to an instant denial of your submission. Please note the Translations & International Support Teams Manager has full discretion on what he approves or denies. This process can sometimes take a considerable amount of time, so it's in your best interest to follow all of the guidelines from the start. If your language pack is denied and then resubmitted, it is placed at the end of the queue.

1. Submissions have to be compatible with the latest version of phpBB. Any missing key will be detected during the upload process and your submission will be automatically denied.

2. Submissions have to be complete. Partial translations are not allowed and will be systematically denied. E-mail text files and imagesets must also be fully translated. Only `search_ignore_words.php` and `search_synonyms.php` are allowed to be untranslated.


3. Language packs can contain five additional files (one mandatory and four optionals) that are not present in the British English language pack: `LICENSE` (mandatory), `README` (optional), `AUTHORS` (optional), `VERSION` (optional) and `CHANGELOG` (optional). They have to be without any file extension and with a capitalized filename, it is case sensitive. You are free to write whatever you want in the `README` file, you can list all the authors and contributors of your language pack in the `AUTHORS` file, you can put the version of your language pack in the `VERSION` file and you can list all the version history in the `CHANGELOG` file. Concerning the `LICENSE` file, it is automatically added during the upload process, you do not have to manually add it. It tells to the user the license used. Language packs inherits phpBB's license [GNU General Public License 2.0](http://www.opensource.org/licenses/gpl-2.0.php "GNU General Public License 2.0"), and no additional or alternative licenses are allowed. These files must be placed in the `language/{iso}/` directory, where is the `iso.txt` file. Any other additional file will be detected during the upload process and your submission will be automatically denied.


4. Submissions must have the following files and structure:

        languagename_versionnumber.zip
           languagename_versionnumber/
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
                       forums.php
                       groups.php
                       index.htm
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
                       admin_activate.txt
                       admin_send_email.txt
                       admin_welcome_activated.txt
                       admin_welcome_inactive.txt
                       coppa_resend_inactive.txt
                       coppa_welcome_inactive.txt
                       email_notify.txt
                       forum_notify.txt
                       group_added.txt
                       group_approved.txt
                       group_request.txt
                       installed.txt
                       newtopic_notify.txt
                       pm_report_closed.txt
                       pm_report_deleted.txt
                       post_approved.txt
                       post_disapproved.txt
                       privmsg_notify.txt
                       profile_send_email.txt
                       profile_send_im.txt
                       report_closed.txt
                       report_deleted.txt
                       topic_approved.txt
                       topic_disapproved.txt
                       topic_notify.txt
                       user_activate.txt
                       user_activate_inactive.txt
                       user_activate_passwd.txt
                       user_reactivate_account.txt
                       user_remind_inactive.txt
                       user_resend_inactive.txt
                       user_welcome.txt
                       user_welcome_inactive.txt
                    mods/
                       index.htm
                    AUTHORS (optional)
                    captcha_qa.php
                    captcha_recaptcha.php
                    CHANGELOG (optional)
                    common.php
                    groups.php
                    help_bbcode.php
                    help_faq.php
                    index.htm
                    install.php
                    iso.txt
                    LICENSE
                    mcp.php
                    memberlist.php
                    posting.php
                    README (optional)
                    search.php
                    search_ignore_words.php
                    search_synonyms.php
                    ucp.php
                    VERSION (optional)
                    viewforum.php
                    viewtopic.php
              styles/
                 prosilver/
                    imageset/
                       {iso}/
                          button_pm_forward.gif
                          button_pm_new.gif
                          button_pm_reply.gif
                          button_topic_locked.gif
                          button_topic_new.gif
                          button_topic_reply.gif
                          icon_contact_pm.gif
                          icon_post_edit.gif
                          icon_post_quote.gif
                          icon_user_online.gif
                          imageset.cfg
                          index.htm
                 subsilver2/
                    imageset/
                       {iso}/
                          button_pm_new.gif
                          button_pm_reply.gif
                          button_topic_locked.gif
                          button_topic_new.gif
                          button_topic_reply.gif
                          icon_contact_aim.gif
                          icon_contact_email.gif
                          icon_contact_icq.gif
                          icon_contact_jabber.gif
                          icon_contact_msnm.gif
                          icon_contact_pm.gif
                          icon_contact_www.gif
                          icon_contact_yahoo.gif
                          icon_post_delete.gif
                          icon_post_edit.gif
                          icon_post_info.gif
                          icon_post_quote.gif
                          icon_post_report.gif
                          icon_user_offline.gif
                          icon_user_online.gif
                          icon_user_profile.gif
                          icon_user_search.gif
                          icon_user_warn.gif
                          imageset.cfg


5. Submissions have to follow as much as possible the [Translation (i18n/L10n) Guidelines](https://area51.phpbb.com/docs/30x/coding-guidelines.html#translation "Translation (i18n/L10n) Guidelines") recommandantions, especially the [Writing style](https://area51.phpbb.com/docs/30x/coding-guidelines.html#writingstyle "Writing style").


6. All the PHP and text files have to be encoding in UTF-8 without BOM. Many modern text editors use this as a default setting, but we recommend checking it in your editor's settings. We recommend you [Notepad++](http://notepad-plus.sourceforge.net/ "Notepad++") or [PSPad](http://www.pspad.com/en/ "PSPad"), both lightweight and free.


7. The translation is mostly your work and you have a right to hold a copyright and names to it.


8. A maximum of 3 links can be included as an author credit in the footer, customisable via the `'TRANSLATION_INFO'` key in `common.php`. Please note that the Translations Manager has complete discretion on what is acceptable as an author credit link.


9. Submissions have to be submitted as a single zip file. For information, the Customisation Database will automatically name `languagename_versionnumber.zip` your uploaded language pack. For example, if a Brazilian Portuguese language pack author uploads an archive named `Brasileiro_1.0.5.zip`, it will be automatically changed to `brazilian_portuguese_1_0_5.zip`.


10. Contribution description in the Customisation Database should be translated into English in addition of your local language. Some administrators can download your translation without speak your language.


11. Contribution screenshot in the Customisation Database should only be the flag of the country whose the language is spoken. For example, the flag of France for the French language.


12. Revision name in the Customisation Database should be left blank for more understanding.


13. The Demo URL in the Customisation Database must be empty, unless you want to put a link to an international community ([officially](https://www.phpbb.com/support/intl/ "officially") listed or not) related to the language of the contribution. For example, http://www.phpbbarabia.com/ as Demo URL concerning the [Arabic language](https://www.phpbb.com/customise/db/translation/arabic/ "Arabic language") is allowed.
