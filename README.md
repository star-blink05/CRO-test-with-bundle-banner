Hello, Thanks to visit here.
This is the CRO focus A/B test with the bundle banner on PDP.
Here is the figma design : https://www.figma.com/design/IxZ8a6IInfEBPYf2k683em/Test-Dev-task?node-id=0-1&p=f&t=cZy0NjQ7WrCL9AfB-0
Here is the Dev Store Link and Password : https://knife-half.myshopify.com/, mutuch

The approach to do A/B testing.
1. Which is better between Convert and Intellegems?
Convert is better. All of the tools has its all benefits. Convert is easy to setup and get the URL. It does A/B test based on the URL parameter so easy.
But for Intellegems it is alittle more complex to setup than Convert. So I recommend here to use the Convert. For the complex group testing or some kind of
complex setup with many groups we can use the Intellegems coz it has more better point in the complex build.
Convert.com is powerful for broader CRO experimentation, but for Shopify-native price, bundle, and offer testing, Intelligems provides tighter integration, cleaner data, and faster execution.
2. Full URL Targeting Rules
 Only on PDP - Rules : URL contains /products/
3. Traffic split and minimum sample size estimate
   Variant : 50%
   Origin : 50%
   Based on session time estimate : 2,000 sessions/day → Test runs ~10–14 days
                                    5,000 sessions/day → Test runs ~4–7 days
4. Primary and secondary success metrics with definitions
   - Primary Metric
     Calculation : Orders ÷ Sessions to PDP -> Conversion Rate (CVR)
     Reason : Direct business impact and statistically stable.
   - Secondary Metrics
     Calculation : Total revenue ÷ total visitors -> Revenue per Visitor (RPV)
                   Revenue ÷ Orders -> Average Order Value (AOV)
                   ATC clicks ÷ PDP sessions -> Add to Cart Rate (Using GTM and GA4
5. How you would QA the test before launch
   Here is the approach to QA before launch. First I will review the origin and variant URLs on the Incognito.
   And confirm the condition if this test only works on the PDP.
   And after that I will check on all devices such as iphone, Android etc. I always using Browser stack here.
6. Any risks or edge cases (e.g. mobile vs desktop split, returning visitors)
   ⚠️ Mobile vs Desktop Behavior : Mobile traffic often converts differently. If traffic volume allows, analyze by device post-test.
   ⚠️ Returning Visitors : Returning users may -> See a different variant, Have cached pricing etc.
                           Mitigation -> Sticky session assignment,Cookie-based bucketing.
   ⚠️ Inventory Fluctuation : Low inventory can skew results. Avoid running during stockouts.
   ⚠️ Seasonality & Promotions : Major sale campaigns, Email promotions, Paid traffic spikes, BFCM or flash sales
