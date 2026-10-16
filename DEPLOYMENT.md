# Review and deployment

This repository now includes the existing Mortgage Mike website under dist/, with the prepared Formspree consultation integration.

## Test status

Local JavaScript syntax and preservation checks passed. The calculator, pre-approval link, headshot and contact section are unchanged. The original headshot file is copied byte-for-byte into dist/assets/.

The cloud proxy blocked the fictional Formspree test before it reached Formspree. Receipt, dashboard recording and notification email delivery have NOT been verified. Test from Chrome with fictional details and confirm the record in Formspree before accepting real leads.

## Integration

HTTPS JSON POST to https://formspree.io/f/meaevvoy. Required name, email, phone, mortgage interest and unchecked affirmative contact consent; honeypot; duplicate-click prevention; timeout and helpful failure response. Success is displayed only after an HTTP success and Formspree ok=true. No sensitive mortgage application fields are included. Privacy notice describes Formspree processing and contact withdrawal.

## Next steps

1. Review and merge this PR into main.
2. Request publication of the merged GitHub source to the existing Sites project appgprj_6acf9b3f20d48191b5b1aaad2684a973 using the normal authorized Sites source and deployment workflow. GitHub merging alone does not publish this Site; it currently has a separate Sites source repository. Do not create a replacement Site or change its audience.
3. Submit fictional information through Chrome, confirm its record in the Formspree dashboard and verify email notifications. Check invalid fields, unchecked consent and failure behavior before accepting real customer leads.

No deployment is performed by this PR.
