# KriTere.com: AdSense guide for a family and kids website

Goal: show ads on www.kritere.com in a way that is safe for children and meets the
rules in Europe (GDPR / ePrivacy) and the USA (COPPA and US state privacy laws).

## Already done

- Offerwall removed for kritere.com.
- Auto ads turned OFF for kritere.com.
- The theme asks Google for non-personalised ads for every visitor.

Two ad spots with the child tag are now in the theme: one before Parents' corner and one
after Our story, both labelled "Advertisement".

## Which settings affect your other sites?

| Where | Applies to |
|---|---|
| Ads → By site → kritere.com | Only kritere.com |
| Blocking controls with **kritere.com** chosen in "Search sites…" | Only kritere.com |
| Blocking controls with **All sites** chosen | All your sites |
| Privacy & messaging → European regulations → **Settings** | All your sites |
| Privacy & messaging → US state regulations → **Settings** | All your sites |
| A GDPR or US message | Only the sites listed in that message |
| Code in the KriTere theme | Only kritere.com |

---

## Step 1: Two ad spots with the child tag

1. AdSense → **Ads → By ad unit → Display ads**.
2. Name: `KriTere 1`, shape: **Responsive** → **Create** → copy the number in `data-ad-slot="…"`.
3. Repeat for `KriTere 2`.
4. Send both numbers to Claude. They will be added to the theme:
   - with Google's child tag (`data-tag-for-age-treatment="1"`), which tells Google the
     visitors may be children: no personalised ads, no remarketing, stricter data limits;
   - labelled "Advertisement";
   - away from Play buttons, trailers, the quiz and the phone play bar, so children don't tap
     them by accident (accidental clicks can also get an AdSense account penalised).
5. The Privacy Policy will then be updated to say the ads are treated as child-directed.

---

## Step 2: Europe (EEA, UK, Switzerland)

The law (GDPR and the ePrivacy rules) requires asking for consent before cookies are used,
**even for non-personalised and child-directed ads**. Your Google consent message does this.

### 2a. Your GDPR message (Privacy & messaging → European regulations)

- Keep the message **published**. It covers 11 sites, including kritere.com.
- Open it and check that kritere.com is in its **Sites** list.
- Leave the rest as it is.

### 2b. European regulations → Settings (affects all your sites)

| Setting | Choose | Why |
|---|---|---|
| Review your ad partners | **Automatically include commonly used ad partners** | You have 1256 partners; above 700 the consent message may not work properly |
| Fallback message | **ON** | Safety net if the consent message fails to show |
| Auto-created messages | **ON** | New sites get a consent message automatically |
| Ask buyers to only show ads with DSA transparency information | **OFF** | Not required of you; Google warns it can cut revenue a lot |
| Check creatives for consent | **ON** | Blocks ads from partners the visitor didn't agree to |
| Check RTB partner creatives for ad partner consent | **ON** | Same, for real-time bidding partners |
| Legitimate interest controls | **Keep included** | Removing them can greatly reduce revenue |
| Enable by default (legitimate interest) | **Leave as it is** | |
| Consent mode | **OFF** | Only needed with Google Analytics or Google Ads tags; KriTere has neither. Turn ON only if another site of yours uses Google Analytics |
| Special feature 2 (scan device characteristics) | **OFF** | Lets ad companies identify devices; not suitable for children |

---

## Step 3: USA

### 3a. COPPA (children under 13)

- Covered by the child tag on the ad spots (step 1) and the non-personalised setting in the
  theme. Nothing to click in AdSense.
- Never place ads inside the games (you don't), and never ask visitors to click ads.

### 3b. Your CPRA / US state message (Privacy & messaging → US state regulations)

- Keep it **published** for kritere.com.

### 3c. US state regulations → Settings (affects all your sites)

| Setting | Choose | Why |
|---|---|---|
| Review your ad partners → Use active ad partners (338) | **Leave as it is** | |
| Manage restricted data processing via ad requests | **Leave OFF** | KriTere already restricts data with the child tag; turning this on would also affect your other sites |

---

## Step 4: Blocking controls for kritere.com only

1. AdSense → **Brand safety → Blocking controls** (or **Blocking controls**).
2. In **"Search sites…"** type **kritere.com** and select it. Check that the page title shows
   kritere.com and not "All sites". If kritere.com isn't listed, add it under **Sites** first.

### Sensitive categories: block all of these

Names may differ slightly in your account:

- Dating
- Gambling & betting, including **social casino games**
- Get rich quick
- Consumer loans
- Drugs & supplements
- Weight loss
- Cosmetic procedures & body modification
- Sexual & reproductive health
- References to sex & sexuality
- Astrology & esoteric
- Politics
- Religion

Optional: **Video games (casual & online)**. Blocking it stops ads for other games, which are
often full of in-app purchases. It lowers revenue, so it's your choice.

### Other blocking controls

| Control | Choose |
|---|---|
| General categories | Nothing to block (lowers revenue, not needed) |
| Advertiser URLs | Optional: add any site you never want advertised on KriTere |
| Ad serving | Leave as it is (account-wide) |
| Authorized Buyers | Leave as it is (account-wide) |

---

## Step 5: Other things to check

1. **ads.txt**: open https://www.kritere.com/ads.txt. It should contain
   `google.com, pub-2373589608434861, DIRECT, f08c47fec0942fa0`.
   If it's missing: Blogger → **Settings → Monetization → Enable custom ads.txt** → paste that
   line → Save. (A wrong or missing ads.txt can stop ads or lower revenue.)
2. **Sites list**: AdSense → **Sites** → kritere.com should show **Ready**.
3. **Offerwall**: AdSense → **Privacy & messaging → Offerwall**: no message lists kritere.com.
4. **Auto ads**: AdSense → **Ads → By site → kritere.com**: Auto ads OFF.
5. **Privacy Policy and Contact pages**: published in Blogger, with your contact email filled in.
6. **Never click your own ads**, and don't ask family or friends to click them.
7. After 1–2 days, open kritere.com on a phone and a computer and check that the two ads appear
   in the right places and don't cover any buttons.

---

## Final checklist

- [x] Two ad units created and added to the theme (KriTere1: 1292405443, KriTere2: 4072154013)
- [ ] GDPR message published and includes kritere.com
- [ ] Ad partners: "Automatically include commonly used ad partners"
- [ ] Fallback message ON, auto-created messages ON
- [ ] DSA transparency OFF, creative consent checks ON
- [ ] Consent mode OFF (unless you use Google Analytics elsewhere)
- [ ] Special feature 2 OFF
- [ ] CPRA message published for kritere.com
- [ ] Sensitive categories blocked for kritere.com only
- [ ] ads.txt correct
- [ ] Offerwall not on kritere.com, Auto ads OFF for kritere.com
- [ ] Privacy Policy and Contact pages published

Sources:
- [AdSense: tag ad requests for age treatment](https://support.google.com/adsense/answer/9009582?hl=en)
- [Google: Tag for age treatment replaces child-directed tags](https://support.google.com/adsense/answer/17042704)
- [AdSense: non-personalised ads](https://support.google.com/adsense/answer/9042142)
- [AdSense: site-level blocking controls](https://support.google.com/adsense/answer/180609?hl=en)
- [Google EU user consent policy](https://www.google.com/about/company/user-consent-policy/)
