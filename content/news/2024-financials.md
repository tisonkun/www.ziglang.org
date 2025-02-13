---
title: "2024 Financial Report and Fundraiser"
mobile_menu_title: "2024 Financials"
date: 2024-01-16T00:00:00.000Z
---

<script src="/js/chartist-1.3.0.umd.js"></script>
<link rel="stylesheet" type="text/css" href="/js/chartist-1.3.0.css">
<style>
.ct-label {
    fill: black;
    color: black;
    font-weight: bold;
}
svg.ct-chart-bar, svg.ct-chart-line{
	overflow: visible;
}
td.description {
    white-space: normal;
}
@media (prefers-color-scheme:dark) {
    .ct-label {
        fill: white;
        color: white;
    }
}
</style>

# 2024 Financial Report and Fundraiser

Zig Software Foundation is a 501(c)(3) non-profit organization which I am proud
to say makes **extremely efficient use of monetary resources**. Unlike many of
our peers, our primary expense is direct payments to contributors for their
enhancements to the Zig project.

Don't take my word for it - let's look at some numbers.

## 2023 Expenditures

<div id="chart-categorized-expenses" style="height: 30em"></div>
<script>
  new Chartist.PieChart(
    '#chart-categorized-expenses',
    {
      series: [
        102000.00,
        14661.35,
        9700.00,
        6068.43,
        10847.6,
        8894.66,
        1060.50,
        308102.61,
      ],
      labels: [
        "Employees",
        "CI & Website",
        "Legal System",
        "Sponsorships",
        "Travel",
        "Taxes",
        "Bank Fees",
        "Contractors",
      ]
    },
    {
        labelPosition: 'outside',
        labelDirection: 'explode'
    }
  );
</script>

<table>
<tr>
<th>Expense Name</th>
<th>2023 Cost</th>
<th>Description</th>
</tr><tr>
<td>Contractors</td>
<td>$308,102.61</td>
<td class="description">Direct compensation to contributors working on Zig at a rate of $60/hour.</td>
</tr><tr>
<td>Employees</td>
<td>$102,000.00</td>
<td class="description">ZSF has one employee which is yours truly, Andrew Kelley, serving the role of 
Lead Software Engineer. My duties as President of Zig Software Foundation are
strictly volunteer work;
I am not compensated for serving on the board of directors. The other two
members of the ZSF board of directors
<a href="https://docs.google.com/document/d/1wPQtJxIgCo7SReJev-H7OZGgYt0k8LqECc4G4QYT0aE">chose my salary</a> to be $159,790 per year, matching
the median salary for a Lead Software Engineer in New York City at the time.
<br><br>
I have never once received my full salary. At the time of writing, I am accepting
$108,000/year (before taxes) and donating the rest to ZSF. In the past I have donated
an even larger portion. In the future I think it would be nice to be fully
compensated.
</td>
</tr><tr>
<td>CI & Website</td>
<td>$14,661.35</td>
<td class="description">Zig has great cross-compiling abilities in part
due to investing in testing infrastructure for different systems. Some of these costs were
one-time costs to purchase machines that sit in our homes and offices while others
are market-rate Hetzner bare metal machines that we run GitHub Actions on.
<br><br>
Some of this cost is for hosting ziglang.org. Since our free AWS credits have expired
we have plans to switch to Fastly which should save about $500/month.
</td>
</tr><tr>
<td>Travel</td>
<td>$10,847.6</td>
<td class="description">In a 2022 meeting, <a href="https://docs.google.com/document/d/1EqyZcd4AKu7Y9Zb_xdE_7q8i-NnqIz1BW8IiJxMX6Xc">the board decided</a>
that the previous year's travel budget successfully helped grow Zig adoption,
and raised the budget from $10,000 to $15,000. In 2023, ZSF spent $10,847
of those allocated funds, increasing Zig's presence in North America (e.g. Seattle, Vancouver) and Europe (e.g. Stockholm, Berlin, Amsterdam) as well as keeping up relationships with likeminded communities like
<a href="https://handmade-seattle.com/">Handmade Seattle</a>.
</td>
</tr><tr>
<td>Legal System</td>
<td>$9,700.00</td>
<td class="description">This is mostly paying our accountant,
<a href="https://www.stradafg.com/">Strada Financial Group</a>, to keep the American
legal system happy and keep our organization tax-exempt, but also includes a payment
to a legal firm to help us
<a href="/news/statement-regarding-zen-programming-language/">regain the Zig trademark in Japan from a trademark troll</a>.
</td>
</tr><tr>
<td>Taxes</td>
<td>$8,894.66</td>
<td class="description">Although ZSF is a tax-exempt organization, employees are still required
to pay income tax.</td>
</tr><tr>
<td>Sponsorships</td>
<td>$6,068.43</td>
<td class="description">The Zig project is mostly comprised of in-house code, however,
it also relies on third party projects. Today, every Zig
installation includes some source files or ported code from
<a href="http://musl.libc.org/">musl libc</a>,
<a href="https://www.mingw-w64.org/">mingw-w64</a>, and others.
ZSF donates money to these projects as a way to say thanks, give back to the ecosystem,
and increase the sustainability of Zig's dependencies.
</td>
</tr><tr>
<td>Bank Fees</td>
<td>$1,060.50</td>
<td class="description">This is a tiny slice of the pie, but every time ZSF
wires money, there is a transaction fee. Our contractors graciously bill
infrequently when possible to help reduce this cost.</td>
<td>
</tr><tr>
<td>Total Expenses</td>
<td>$461,335.15</td>
</tr>
</table>

**We spent 92% of our money in 2023 on paying contributors for their time.**

So far so good. You can see we've been hard at work spending our esteemed
donors' money on advancing the [mission statement](/zsf/#mission-statement).

However, if we look at the trend of donations over time for the year 2023, we
see overall a slow decline. This is likely due to the fact that we have slacked
off on *asking for money*.

## 2023 Donations Per Month

<div id="chart-donations-over-time" style="height: 30em"></div>
<script>
  new Chartist.LineChart(
    '#chart-donations-over-time',
    {
      labels: ["Jan", "Feb", "Mar", "Apr", "May", "Jun", "Jul", "Aug", "Sep", "Oct", "Nov", "Dec"],
      series: [[30860.52,27666.32,24618.06,17682.71,18499.45,18604.38,19719.44,20641.36,21068.52,27768.91,25648.49,16913.57]]
    },
    {
      low: 0,
      showArea: true,
      axisY: {
        labelInterpolationFnc: function(n) {
            return Intl.NumberFormat('en-US', {
                style: 'currency',
                currency: 'USD',
                maximumFractionDigits: 0
            }).format(n);
        }
      },
    }
  );
</script>

Meanwhile, **user activity has skyrocketed**. A rapidly increasing user base
is adding Zig to their software stacks, filing issues, sending pull requests,
asking for help, and shipping software that depends on Zig.

## New GitHub Issues Per Month

<div id="chart-issues" style="height: 30em"></div>
<script>
  new Chartist.LineChart(
    '#chart-issues',
    {
        series: [{ data: [
{ x: new Date("Nov 1 2015"), y: 0 },
{ x: new Date("Dec 1 2015"), y: 30 },
{ x: new Date("Jan 1 2016"), y: 37 },
{ x: new Date("Feb 1 2016"), y: 49 },
{ x: new Date("Mar 1 2016"), y: 5 },
{ x: new Date("Apr 1 2016"), y: 6 },
{ x: new Date("May 1 2016"), y: 13 },
{ x: new Date("Jun 1 2016"), y: 2 },
{ x: new Date("Jul 1 2016"), y: 1 },
{ x: new Date("Aug 1 2016"), y: 12 },
{ x: new Date("Sep 1 2016"), y: 14 },
{ x: new Date("Oct 1 2016"), y: 16 },
{ x: new Date("Nov 1 2016"), y: 6 },
{ x: new Date("Dec 1 2016"), y: 3 },
{ x: new Date("Jan 1 2017"), y: 2 },
{ x: new Date("Feb 1 2017"), y: 41 },
{ x: new Date("Mar 1 2017"), y: 9 },
{ x: new Date("Apr 1 2017"), y: 51 },
{ x: new Date("May 1 2017"), y: 48 },
{ x: new Date("Jun 1 2017"), y: 17 },
{ x: new Date("Jul 1 2017"), y: 15 },
{ x: new Date("Aug 1 2017"), y: 8 },
{ x: new Date("Sep 1 2017"), y: 50 },
{ x: new Date("Oct 1 2017"), y: 51 },
{ x: new Date("Nov 1 2017"), y: 59 },
{ x: new Date("Dec 1 2017"), y: 39 },
{ x: new Date("Jan 1 2018"), y: 24 },
{ x: new Date("Feb 1 2018"), y: 67 },
{ x: new Date("Mar 1 2018"), y: 44 },
{ x: new Date("Apr 1 2018"), y: 64 },
{ x: new Date("May 1 2018"), y: 66 },
{ x: new Date("Jun 1 2018"), y: 65 },
{ x: new Date("Jul 1 2018"), y: 78 },
{ x: new Date("Aug 1 2018"), y: 96 },
{ x: new Date("Sep 1 2018"), y: 83 },
{ x: new Date("Oct 1 2018"), y: 105 },
{ x: new Date("Nov 1 2018"), y: 46 },
{ x: new Date("Dec 1 2018"), y: 73 },
{ x: new Date("Jan 1 2019"), y: 28 },
{ x: new Date("Feb 1 2019"), y: 55 },
{ x: new Date("Mar 1 2019"), y: 64 },
{ x: new Date("Apr 1 2019"), y: 121 },
{ x: new Date("May 1 2019"), y: 111 },
{ x: new Date("Jun 1 2019"), y: 102 },
{ x: new Date("Jul 1 2019"), y: 134 },
{ x: new Date("Aug 1 2019"), y: 121 },
{ x: new Date("Sep 1 2019"), y: 102 },
{ x: new Date("Oct 1 2019"), y: 141 },
{ x: new Date("Nov 1 2019"), y: 135 },
{ x: new Date("Dec 1 2019"), y: 115 },
{ x: new Date("Jan 1 2020"), y: 138 },
{ x: new Date("Feb 1 2020"), y: 147 },
{ x: new Date("Mar 1 2020"), y: 156 },
{ x: new Date("Apr 1 2020"), y: 140 },
{ x: new Date("May 1 2020"), y: 172 },
{ x: new Date("Jun 1 2020"), y: 140 },
{ x: new Date("Jul 1 2020"), y: 144 },
{ x: new Date("Aug 1 2020"), y: 103 },
{ x: new Date("Sep 1 2020"), y: 127 },
{ x: new Date("Oct 1 2020"), y: 170 },
{ x: new Date("Nov 1 2020"), y: 218 },
{ x: new Date("Dec 1 2020"), y: 174 },
{ x: new Date("Jan 1 2021"), y: 170 },
{ x: new Date("Feb 1 2021"), y: 130 },
{ x: new Date("Mar 1 2021"), y: 124 },
{ x: new Date("Apr 1 2021"), y: 127 },
{ x: new Date("May 1 2021"), y: 99 },
{ x: new Date("Jun 1 2021"), y: 152 },
{ x: new Date("Jul 1 2021"), y: 123 },
{ x: new Date("Aug 1 2021"), y: 98 },
{ x: new Date("Sep 1 2021"), y: 97 },
{ x: new Date("Oct 1 2021"), y: 95 },
{ x: new Date("Nov 1 2021"), y: 68 },
{ x: new Date("Dec 1 2021"), y: 77 },
{ x: new Date("Jan 1 2022"), y: 115 },
{ x: new Date("Feb 1 2022"), y: 113 },
{ x: new Date("Mar 1 2022"), y: 102 },
{ x: new Date("Apr 1 2022"), y: 122 },
{ x: new Date("May 1 2022"), y: 87 },
{ x: new Date("Jun 1 2022"), y: 85 },
{ x: new Date("Jul 1 2022"), y: 113 },
{ x: new Date("Aug 1 2022"), y: 170 },
{ x: new Date("Sep 1 2022"), y: 243 },
{ x: new Date("Oct 1 2022"), y: 173 },
{ x: new Date("Nov 1 2022"), y: 226 },
{ x: new Date("Dec 1 2022"), y: 191 },
{ x: new Date("Jan 1 2023"), y: 202 },
{ x: new Date("Feb 1 2023"), y: 173 },
{ x: new Date("Mar 1 2023"), y: 120 },
{ x: new Date("Apr 1 2023"), y: 191 },
{ x: new Date("May 1 2023"), y: 171 },
{ x: new Date("Jun 1 2023"), y: 158 },
{ x: new Date("Jul 1 2023"), y: 173 },
{ x: new Date("Aug 1 2023"), y: 202 },
{ x: new Date("Sep 1 2023"), y: 187 },
{ x: new Date("Oct 1 2023"), y: 188 },
{ x: new Date("Nov 1 2023"), y: 224 },
{ x: new Date("Dec 1 2023"), y: 138 },
{ x: new Date("Jan 1 2024"), y: 145 }
    ]}]},
    {
      low: 0,
      showArea: true,
      axisX: {
        type: Chartist.FixedScaleAxis,
        divisor: 12,
        labelInterpolationFnc: function(value) {
          return new Date(value).toLocaleString(undefined, {
            year: 'numeric',
            month: 'short',
          });
        }
      }
    }
  );
</script>

<table style="float:left; padding-right: 2em">
<tr>
<th colspan="2">Average time to close issues</th>
</tr><tr>
<td>All Time</td>
<td>5 months</td>
</tr><tr>
<td>Past Year</td>
<td>7 months</td>
</tr><tr>
<td>Past Month</td>
<td>4 months</td>
</tr>
</table>

<table>
<tr>
<th colspan="2">Average time to close pull requests</th>
</tr><tr>
<td>All Time</td>
<td>12 days</td>
</tr><tr>
<td>Past Year</td>
<td>18 days</td>
</tr><tr>
<td>Past Month</td>
<td>about 1 month</td>
</tr>
</table>

Source: [Repo Trends](https://www.repotrends.com/ziglang/zig)

## Total GitHub Stars

<div id="chart-the-stars" style="height: 30em"></div>
<script>
  new Chartist.LineChart(
    '#chart-the-stars',
    {
      series: [{
        data: [
            {x: new Date("Fri Jan 08 2016 02:38:00 GMT-0700 (Mountain Standard Time)"), y: 0},
            {x: new Date("Mon Oct 15 2018 03:43:08 GMT-0700 (Mountain Standard Time)"), y: 1800},
            {x: new Date("Mon Sep 30 2019 15:01:31 GMT-0700 (Mountain Standard Time)"), y: 3690},
            {x: new Date("Fri Jul 03 2020 09:03:02 GMT-0700 (Mountain Standard Time)"), y: 5550},
            {x: new Date("Sun Jan 24 2021 13:25:39 GMT-0700 (Mountain Standard Time)"), y: 7410},
            {x: new Date("Sat Jul 24 2021 12:34:12 GMT-0700 (Mountain Standard Time)"), y: 9300},
            {x: new Date("Wed Dec 22 2021 07:22:25 GMT-0700 (Mountain Standard Time)"), y: 11160},
            {x: new Date("Sun Apr 24 2022 08:18:33 GMT-0700 (Mountain Standard Time)"), y: 13020},
            {x: new Date("Mon Jul 11 2022 18:42:09 GMT-0700 (Mountain Standard Time)"), y: 14910},
            {x: new Date("Mon Aug 29 2022 05:54:19 GMT-0700 (Mountain Standard Time)"), y: 16770},
            {x: new Date("Wed Dec 28 2022 16:11:02 GMT-0700 (Mountain Standard Time)"), y: 18630},
            {x: new Date("Sun Apr 02 2023 13:17:57 GMT-0700 (Mountain Standard Time)"), y: 20520},
            {x: new Date("Wed Jun 07 2023 07:50:41 GMT-0700 (Mountain Standard Time)"), y: 22380},
            {x: new Date("Mon Aug 07 2023 22:53:49 GMT-0700 (Mountain Standard Time)"), y: 24240},
            {x: new Date("Mon Oct 09 2023 09:06:48 GMT-0700 (Mountain Standard Time)"), y: 26130},
            {x: new Date("Wed Jan 10 2024 18:18:32 GMT-0700 (Mountain Standard Time)"), y: 27990},
            {x: new Date("Tue Jan 16 2024 19:45:54 GMT-0700 (Mountain Standard Time)"), y: 28123},
        ]
      }]
    },
    {
      low: 0,
      showArea: true,
      axisX: {
        type: Chartist.FixedScaleAxis,
        divisor: 8,
        labelInterpolationFnc: function(value) {
          return new Date(value).toLocaleString(undefined, {
            year: 'numeric',
            month: 'short',
            day: 'numeric'
          });
        }
      }
    }
  );
</script>

In response to this rising demand, we
[added incredible new members to the Zig core team](/news/welcome-jacob-young/).
Thanks to the income that was available to us in 2023, we were able to offer
new contracts.

## 2023 Income

<div id="chart-categorized-income" style="height: 30em"></div>
<script>
  new Chartist.PieChart(
    '#chart-categorized-income',
    {
      series: [
        19851.42,
        184800,
        22000,
        58666.67,
        15000.00,
        145462.88,
        8710.76,
      ],
      labels: [
        "Benevity",
        "Uber Support Contract",
        "TigerBeetle",
        "Bun",
        "Pex",
        "GitHub Sponsors",
        "Individuals",
      ]
    },
    {
        labelPosition: 'outside',
        labelDirection: 'explode'
    }
  );
</script>

<table>
<tr>
<th>Income Name</th>
<th>2023 Amount</th>
<th>Description</th>
</tr><tr>
<td>Uber Support Contract</td>
<td>$184,800.00</td>
<td class="description">Uber has wisely agreed to a support contract since
<a href="https://www.youtube.com/watch?v=SCj2J3HcEfc">they use the Zig toolchain</a>
and want a guaranteed Service-Level Agreement if they run into any bugs while using it.
Other companies are invited to follow in their footsteps and obtain a ZSF support contract in
order to guarantee speedy response when encountering a bug while using Zig.
</td>
</tr><tr>
<td>GitHub Sponsors</td>
<td>$145,462.88</td>
<td class="description"><a href="https://github.com/sponsors/ziglang">Zig on GitHub Sponsors</a>. This category contains a numerous amount of both individuals and companies. It's pretty convenient
for both ZSF and donors, as long as Microsoft keeps being cool about it. Hopefully they don't
alter the deal anytime soon. We lost a lot of donors when they dropped PayPal support.</td>
</tr><tr>
<td>Bun</td>
<td>$58,666.67</td>
<td class="description"><a href="https://bun.sh/">Bun</a> is a
fast JavaScript all-in-one toolkit built using the Zig programming language. The company
behind Bun sponsors ZSF in order to ensure that the tech stack they depend on
continues to flourish, improve, and become more widely adopted.</td>
</tr><tr>
<td>TigerBeetle</td>
<td>$22,000.00</td>
<td class="description"><a href="https://tigerbeetle.com/">TigerBeetle</a> is a database company
whose product is built on the Zig programming language and likewise sponsors ZSF. It's
good business practice to keep your software supply chain healthy.
</td>
</tr><tr>
<td>Benevity</td>
<td>$19,851.42</td>
<td class="description">Benevity helps us collect company-matched donations from employees.
This category contains a number of individuals.</td>
</tr><tr>
<td>Pex</td>
<td>$15,000.00</td>
<td class="description"><a href="https://pex.com/">Pex</a> is a company whose product helps
enable the fair and transparent use of copyrighted content.
</td>
</tr><tr>
<td>Individuals</td>
<td>$8,710.76</td>
<td class="description">This category contains people who donate via paper checks,
<a href="https://www.every.org/zig-software-foundation-inc/">via every.org</a>, or via
UK Online Giving Foundation.</td>
</tr><tr>
<td>Total Income</td>
<td>$454,491.73</td>
</tr>
</table>

However, with our current level of recurring income, we will not be able to renew
everyone's contracts, nor offer new contracts to Zig core team members.

## A Plea for Donations

We have extremely talented Zig core team members who want to renew their
contracts, and others who are interested to start getting paid for their
valuable work for the first time.

In order to do this, **we need more recurring donations**. I for one do not enjoy
asking for money, but in the interest of our users and contributors, it would
be irresponsible not to.

**Please sign up for a monthly donation** if you can. Our preferred donation method
is [via Every.org](https://www.every.org/zig-software-foundation-inc/f/help-zig-stay-indepe).
A fellow 501(c)(3) non-profit, they seamlessly manage gift receipts, and are not 
pivoting to AI [like GitHub is currently doing](https://github.blog/2023-11-08-universe-2023-copilot-transforms-github-into-the-ai-powered-developer-platform/), which frankly scares the shit
out of us.

<div id="every-donate-btn">
  <a href="https://www.every.org/zig-software-foundation-inc?utm_campaign=2024_financials#/donate">Donate</a>
  <script>
    function createWidget() {
      everyDotOrgDonateButton.createButton({
        selector: "#every-donate-btn",
        nonprofitSlug: "zig-software-foundation-inc",
        fundraiserSlug: "help-zig-stay-indepe",
        fontSize: "32px",
        label: "Sponsor"
      });
      everyDotOrgDonateButton.createWidget({
        selector: "#every-donate-btn",
        nonprofitSlug: "zig-software-foundation-inc",
        fundraiserSlug: "help-zig-stay-indepe",
        defaultDonationAmount: 10,
        defaultFrequency: 'monthly'
      });
    }
    if (window.everyDotOrgDonateButton) {
      createWidget();
    } else {
      document.getElementById("every-donate-btn-js-nav").addEventListener('load', createWidget);
    }
  </script>
</div>

<table>
<tr>
<th>Companies</th><td class="description">Contact us to get your logo on ziglang.org in exchange for a monthly donation.</td>
</tr><tr>
<th>Employees</th><td class="description">Check if your company matches donations to charities such as Zig Software Foundation. That 2x multiplier makes a huge difference. We're already in the system.</td>
</tr><tr>
<th>Venture Capitalists</th><td class="description">We are aware of a few startups betting on Zig as their language and toolchain of choice to build tomorrow's critical infrastructure. Helping the Zig Software Foundation reach v1.0 faster is one of the most efficient uses of capital you can make to boost your portfolio.</td>
</tr><tr>
<th>Individuals</th><td class="description">Can you spare $5-10 per month? This is our favorite
kind of donation because it helps diversify ZSF's income, keeping us free from undue influence
from any single party.</td>
</tr>
</table>

Huge thanks to all who graciously donate funds to our cause. Together we serve the users!
