# KriTere guides (Blogger posts)

Two posts for the "Game night guides" section on the homepage. Every rule in them comes from
the game repositories (dgm-game: docs/GCD.md and the in-game guide; kaj-game: docs/KAJ-v1-scope.md,
the in-game tutorial and src/engine/constants.ts).

## How to publish each post

1. Blogger → **Posts → New post**.
2. Switch the editor to **HTML view** (the `< >` icon) and paste the whole file.
3. Title (exactly):
   - `how-to-play-dont-get-mad.html` → **How to Play Don't Get Mad!: Rules, Tips and Tricks**
   - `how-to-play-kris-anns-journey.html` → **How to Play Kris Ann's Journey: Rules, Travellers and Tips**
4. In **Post settings** on the right:
   - **Labels** (type them exactly, separated by commas):
     - Don't Get Mad! guide: `Featured, Don't Get Mad!, Rules`
     - Kris Ann's Journey guide: `Featured, Kris Ann's Journey, Rules`
   - **Permalink → Custom permalink:** `how-to-play-dont-get-mad` or `how-to-play-kris-anns-journey`
   - **Search description** (important: it becomes the post's description in Google and on social networks):
     - Don't Get Mad!: `How to play Don't Get Mad!, the free family dice race game: rolling a 6 to start, lanterns, the Bog, Bonus cards, bumping and how to win. Rules and tips.`
     - Kris Ann's Journey: `How to play Kris Ann's Journey, the free geography board game and trivia quiz: travellers, points, tickets, quizzes, businesses, citizenship and tips to win.`
   - **Comments:** "Hide" (keeps the site safe for children).
5. **Publish** (any date). The first picture in each post becomes its picture on the homepage.

## How "Featured" works

- The homepage shows the **2 newest posts with the label `Featured`**. Dates and addresses don't matter.
- **To feature a new guide** (for example next year's updated rules): add the label `Featured` to the new
  post, and remove it from the guide it replaces. Nothing to change in the theme.
- A post with the label `Kris Ann's Journey` gets the teal card; every other post gets the yellow card.
- Posts without `Featured` appear only under **Other guides** (all posts, newest first, 6 per page by
  default; change it in Blogger → Settings → Posts → "Max posts shown on main page") and under
  **You may also like** at the end of each guide.

## What Google gets from every post (added by the theme)

You only paste the article. The theme adds the rest when Blogger builds the page:

- `<title>`: the post title + " | KriTere"
- meta description, Open Graph and X (Twitter) tags: from the post's **Search description**
- canonical address, `robots: index, follow`
- share image: the post's first picture (or the KriTere share image)
- BlogPosting data: title, description, dates, picture, keywords (labels), publisher,
  and which game it is about (from the label `Don't Get Mad!` or `Kris Ann's Journey`)
- breadcrumb: KriTere › Game night guides › post title

To check a published post: open https://search.google.com/test/rich-results and paste its address.
