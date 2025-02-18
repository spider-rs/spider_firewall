# spider_firewall

A shield to prevent bad websites from messing up your system.

`cargo add spider_firewall`

```rust
use spider_firewall::is_bad_website_url;

fn main() {
    let domain = url::Url::parse("https://badwebsite.com").expect("parse");
    let blocked = is_bad_website_url(&domain);
}
```

The build can take up to 5-10 minutes to build locally.