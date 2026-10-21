# Order Confirmation and Delivery Detail Message Templates

Adapt these drafts to the merchant's real order, delivery process, customer consent, approved WhatsApp templates, and local requirements. Asking for additional address or location information should be optional where possible and limited to what the courier actually needs. Do not claim a specific legal address requirement without current official verification.

## Arabic: order confirmation

مرحبًا {{customer_name}}، استلمنا طلبك رقم {{order_number}} من {{store_name}} بإجمالي {{order_total}} {{currency}}. هل تؤكد رغبتك في استلام الطلب؟

{{confirm_button}} · {{cancel_button}}

## English: order confirmation

Hi {{customer_name}}, we received order {{order_number}} from {{store_name}} for {{order_total}} {{currency}}. Would you like to confirm that you still want the delivery?

{{confirm_button}} · {{cancel_button}}

## Delivery details, only if needed

Arabic: لتنسيق التوصيل، يمكنك مراجعة العنوان المسجل أو إرسال التعديل اللازم هنا: {{address_summary}}. لا ترسل بيانات الدفع أو كلمات المرور عبر المحادثة.

English: To coordinate delivery, you can review the saved address or send a correction here: {{address_summary}}. Do not send payment details or passwords in chat.

## Before enabling

- Confirm customer opt-in, message category/template approval, and current provider pricing.
- Confirm order amount, currency, delivery promise, cancellation path, and escalation contact.
- Request only necessary delivery details; explain purpose and provide an alternative support path.
- Test the flow internally and measure confirmation, cancellation, delivery, and complaint rates using a defined baseline.
- Do not promise a reduction in returns, cancellations, or costs.

