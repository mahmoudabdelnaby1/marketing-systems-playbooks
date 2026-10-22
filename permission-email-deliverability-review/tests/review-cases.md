# Email Review Cases

1. **Record exists, message fails:** Report DNS configuration and message authentication separately; identify the tested provider and message.
2. **Authentication passes, alignment is unclear:** Do not call DMARC aligned until the relevant authenticated identifier matches under the published alignment mode.
3. **Gmail bulk rule:** Apply the additional Gmail requirements only when the sender exceeds 5,000 messages per day to Gmail personal accounts; distinguish marketing/subscribed messages from transactional mail.
4. **Provider mismatch:** Do not apply Yahoo's unsubscribe acceptance or Outlook.com consumer rules to another service without checking its own guidance.
5. **Header shared publicly:** Stop and sanitize recipient data, message body, identifiers, and tokens before sharing.
6. **A test reaches inbox:** Record the single test result; do not infer a delivery guarantee for all recipients, providers, or future sends.
7. **Open rate improves:** Treat it as a provider/tool-reported engagement metric only; do not present it as proof that mail reached an inbox.

Pass condition: a second reviewer can reproduce the finding from dated evidence and identify the precise provider rule without confusing configuration, authentication, alignment, and placement.
