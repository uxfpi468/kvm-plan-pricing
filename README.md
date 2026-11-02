# unmanaged linux vps: what a $21.99/year KVM plan really gets you, plus renewal pricing and the fine print worth knowing before you order

An unmanaged Linux VPS means you rent a server with full root access and handle the software side yourself — the provider keeps the hardware, network and virtualization layer running, and everything from installing the OS stack to firewall rules and backups is on you. It's the cheapest way to get a real Linux machine on the public internet, and among the current options, RackNerd's KVM specials sit at the very low end of the price range: five annual plans from $21.99/year, each with KVM virtualization, full root access, a dedicated IPv4 and a 1Gbps port.

That price raises an obvious question — is it a teaser rate that doubles at renewal? Short answer: no, and that's verifiable on the official specials page FAQ, which states the specials are "lifetime recurring. You can renew at the same rate for as long as you decide to keep the service." The rest of this article walks through the plans, the real multi-year cost, the limitations that only show up in the terms, and who should honestly buy something else.

> **Quick pick:** for most self-hosting projects — a small website, Docker containers, a personal VPN, an API service — the **2 GB KVM VPS at $35.99/year** (2 vCPU, 35 GB SSD, 5 TB traffic) is the sensible default. Lighter one-page or VPN-only uses get by on the 1 GB plan at $21.99/year. 👉 [Order the 2 GB plan at $35.99/year](https://my.racknerd.com/cart.php?a=add&pid=953&aff=11397)

## What "unmanaged" actually means — and who shouldn't buy one

Unmanaged is a support boundary, not a quality label. RackNerd's staff will answer tickets around infrastructure problems — the VPS won't boot, the network is down, the node is degraded — around the clock, and the general response time on tickets runs around twenty minutes based on published accounts. What they won't do is log into your server to fix your Nginx config at 3 a.m., harden your SSH setup, or restore a backup you never took.

A third-party review puts the boundary bluntly: if you don't know what `apt` does, or you need someone to fix your web server config in the middle of the night, this category isn't the right fit — the price reflects that.

So who should look elsewhere? If you want someone else to handle OS patching and server administration, you're in the market for a managed VPS, which costs more by definition: Hostwinds, for example, lists managed Linux VPS plans starting at $7.14/month as of September 2026. That's roughly $85+ per year versus RackNerd's $21.99 — the gap is exactly what you're paying for when you buy management. If you can hold your own at a Linux shell, the unmanaged route is where the value is.

## The current plan lineup

RackNerd's specials page currently shows five annual KVM VPS plans. All of them include KVM virtualization, full root access, one dedicated IPv4 address, a 1Gbps network port, RAID-10 SSD storage, and deployment across multiple datacenter locations. These are annual-only — the specials don't have a monthly billing option.

| 套餐 | vCPU / 内存 | SSD 存储 | 月流量 | 年付价格 | 订购 |
| --- | --- | --- | --- | --- | --- |
| 1 GB KVM VPS | 1 vCPU / 1 GB | 20 GB | 3 TB | **$21.99**（≈$1.83/月） | [ 订购 1 GB 套餐](https://my.racknerd.com/cart.php?a=add&pid=952&aff=11397) |
| 2 GB KVM VPS | 2 vCPU / 2 GB | 35 GB | 5 TB | **$35.99**（≈$3.00/月） | [ 订购 2 GB 套餐](https://my.racknerd.com/cart.php?a=add&pid=953&aff=11397) |
| 4 GB KVM VPS | 3 vCPU / 4 GB | 60 GB | 7 TB | **$59.99**（≈$5.00/月） | [ 订购 4 GB 套餐](https://my.racknerd.com/cart.php?a=add&pid=954&aff=11397) |
| 6 GB KVM VPS | 6 vCPU / 6 GB | 100 GB | 12 TB | **$89.99**（≈$7.50/月） | [ 订购 6 GB 套餐](https://my.racknerd.com/cart.php?a=add&pid=955&aff=11397) |
| 8 GB KVM VPS | 7 vCPU / 8 GB | 150 GB | 20 TB | **$119.99**（≈$10.00/月） | [ 订购 8 GB 套餐](https://my.racknerd.com/cart.php?a=add&pid=956&aff=11397) |

Separately from the specials, RackNerd sells a standard KVM VPS line billed monthly, with smaller and larger options: a 512 MB plan at $26.99/year, then 1 GB ($17.99/mo), 2 GB ($20.59/mo), 4 GB ($24.59/mo), 6 GB ($27.59/mo), 8 GB ($36.59/mo) and 12 GB ($55.99/mo), with proportionally larger storage and traffic allocations. If you want to trial a server before committing to a year, the monthly line is where you'd do it — the specials are annual-pay only.

## Renewal pricing: the question everyone asks first

RackNerd's specials renew at the same price you paid. This is stated directly in the official FAQ, and it's the single most important fact about these plans, because the cheap-VPS market has a well-known pattern of low first-year prices followed by steep renewal jumps.

Run the multi-year math on the 2 GB plan: $35.99 in year one, $35.99 in year two, $35.99 in year three — $107.97 total over three years, or about $3.00/month the whole way through. Compare that with the classic "first year $10, renewal $60" structure that some hosts run, where the same three years cost well over $130. Over a typical multi-year hosting lifetime, the renewal terms matter more than the sticker price.

One caveat worth knowing: the lifetime-renewal guarantee applies to the specials themselves. RackNerd also runs bigger seasonal promotions — Black Friday 2025 dropped a 1 GB plan to $10.60/year and an 8 GB plan to $62.49/year — and those deals are stock-limited and disappear once sold out. If you land one of those, the same renewal rule applies to it too. 👉 [Check RackNerd's current specials and renewal terms](https://bit.ly/RacKnerd)

Renewal itself is manual by default: an invoice is generated 14 days before expiry and emailed to you, and you pay it from the client area. Auto-payment exists as an opt-in if you'd rather not think about it. There's also a grace period of a few days to a week after expiry where the server is suspended but data is retained, with reminder emails along the way — service is only reclaimed after that window closes.

## The fine print: no refunds, upgrade paths, and traffic overage

This is the part most roundup articles skip, and it should genuinely influence your decision.

**There is no standard refund.** RackNerd's services are sold on a no-refund basis once purchased. There's no 30-day money-back window here. If that's a dealbreaker for you, the monthly standard line is the lower-risk way to test the waters, since your exposure is one month's fee. Separately from refunds, an SLA credit exists for downtime, but you have to claim it within 30 days of the incident.

**Upgrades between plan types don't happen in place.** You can't flip a specials VPS into a different product through a setting — moving to a different plan or a different datacenter means ordering a new server and migrating your data (or opening a ticket to arrange it). And here's the trap: if you "upgrade" from an annual special into the standard monthly line, your renewal price resets to the standard monthly pricing, and the locked-in annual rate is gone. If the locked price matters to you, buy the plan size you expect to need rather than planning to upgrade into it later.

**Traffic overage is billed per GB.** The monthly allocations are generous — 3 TB on the smallest plan, 20 TB on the largest — but going over isn't free. Match the allocation to your actual traffic rather than assuming "unmetered," because it isn't.

## What you can actually run on it

Every specials plan boots your choice of CentOS, Rocky Linux, AlmaLinux, Fedora, Debian, or Ubuntu, and custom ISO installs are available on request through a support ticket. The company's control panel (ctrl) handles reinstalls, an HTML5 VNC console, root password resets, and a firewall for inbound filtering — and it has a public interactive demo you can click through without an account, which is a rare bit of transparency for a host at this price.

One-click apps cover the usual self-hosting suspects: WordPress stacks, Docker via Portainer, n8n, Coolify, and several AI tools including Ollama, AnythingLLM and LibreChat. The memory requirements are stated officially and worth checking against the plan table above before you order:

- **OpenClaw** needs at least 8 GB RAM — that's the top plan only
- **Hermes Agent, AnythingLLM, Ollama, LibreChat** want at least 4 GB
- **n8n and Coolify** run comfortably from 2 GB

In other words, if running a local LLM stack is your goal, the $21.99 plan won't cut it; the 4 GB plan at $59.99/year is the entry point, and 👉 [the 8 GB plan at $119.99/year](https://my.racknerd.com/cart.php?a=add&pid=956&aff=11397) is what OpenClaw actually requires.

## Picking a datacenter

RackNerd operates roughly twenty datacenters across North America, Europe and Asia — Los Angeles, New York, Chicago, Dallas, Seattle, San Jose, Atlanta, Ashburn, Toronto, Amsterdam, London, Dublin, Strasbourg and others. Two practical notes: there's no Singapore location, and the LA location with Asia-optimized routing is generally the lowest-latency choice for visitors in China (San Jose is the runner-up), though these are standard routes without premium CN2 GIA lines. For everyone else, pick whichever datacenter sits closest to your users.

A small perk on the standard line: the Los Angeles and France locations support up to 100 free IPv6 addresses, requested via ticket.

## FAQ

**Is a $21.99/year VPS too cheap to be reliable?** Cheap, yes; unreliable, not demonstrably. RackNerd has made the Inc. 5000 list four years running (ranking #3,693 nationally in 2026) and runs KVM virtualization on RAID-10 SSDs rather than the oversold OpenVZ setups that gave cheap VPS a bad name. The realistic weaknesses reported by users are occasional evening-hour bandwidth fluctuation on some East Coast nodes and the bare-bones support scope that "unmanaged" implies.

**Can I get a monthly option to try it out?** Not on the specials — those are annual-pay only. The standard KVM line bills monthly (1 GB at $17.99/month and up), so a one-month trial there costs about half a year of the cheapest special.

**What happens if I stop paying?** The server is suspended, data is kept during a grace period of a few days to a week while reminder emails go out, and the service is reclaimed only after that period ends.

**Do the specials include an IPv4 address?** Yes — one dedicated IPv4 per plan, plus full root access and the 1Gbps port.

## Before you click order

Match the plan to the job: VPN, a static site or Linux practice → 1 GB at $21.99/year is plenty; general self-hosting and Docker → 2 GB at $35.99/year; a full web stack with database → 4 GB; AI tooling → 4 GB minimum, 8 GB for the heaviest of it. Confirm you're comfortable with two things first: the no-refund policy (all sales final once purchased) and the fact that annual specials can't be upgraded in place without giving up the locked rate. If both are fine, 👉 [RackNerd's current specials page has the full lineup](https://bit.ly/RacKnerd) — and with a fall giveaway running through November 30 (no purchase required), it's not a bad moment to be looking.
