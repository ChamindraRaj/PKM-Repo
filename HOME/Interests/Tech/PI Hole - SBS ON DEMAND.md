SBS On Demand is an **absolute menagerie** of telemetry, and despite my experience in this stuff, it took a good couple hours of trial and error for it to work.

If you use my [tick lists](https://firebog.net), you'll have these domains already blocked:

    thefilter.com
    www.thefilter.com
    api211.thefilter.com
    d16s8pqtk4uodx.cloudfront.net
    d20i5e3rqc90ne.cloudfront.net
    d29usylhdk1xyu.cloudfront.net
    d3hmp0045zy3cs.cloudfront.net
    docj27ko03fnu.cloudfront.net
    rpxnow.com
    nexus.ensighten.com

The domains I've found are required for SBS On Demand include:

    www.sbs.com.au
    sbs.com.au
    api.sbs.com.au
    media.sbs.com.au
    resources.sbs.com.au
    videocdn-sbs.akamaized.net
    sbsvodns-vh.akamaihd.net
    link.theplatform.com
    e7065.e2.akamaiedge.net
    a463.w10.akamai.net
    a790.w16.akamai.net

Most of them shouldn't be blocked; this is just a C/P list from my Top Domains API exclusions (because I don't like known domains appearing in my Top Domains list on the dashboard).

Do bear in mind that when you log in using your account, you'll get a loading spinner. When that spinner finishes, the login prompt won't go away, so just refresh the page and it'll work fine.