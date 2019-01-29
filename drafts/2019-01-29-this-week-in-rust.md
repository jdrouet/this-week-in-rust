Title: This Week in Rust 271
Number: 271
Date: 2019-01-29
Category: This Week in Rust

Hello and welcome to another issue of *This Week in Rust*!
[Rust](http://rust-lang.org) is a systems language pursuing the trifecta: safety, concurrency, and speed.
This is a weekly summary of its progress and community.
Want something mentioned? Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) or [send us a pull request](https://github.com/cmr/this-week-in-rust).
Want to get involved? [We love contributions](https://github.com/rust-lang/rust/blob/master/CONTRIBUTING.md).

*This Week in Rust* is openly developed [on GitHub](https://github.com/cmr/this-week-in-rust).
If you find any errors in this week's issue, [please submit a PR](https://github.com/cmr/this-week-in-rust/pulls).

# Updates from Rust Community

## News & Blog Posts

# Crate of the Week

This week's crate is [typetag](https://github.com/dtolnay/typetag), a small crate to allow for serde trait objects. Thanks to [Christopher Durham](https://users.rust-lang.org/t/crate-of-the-week/2704/481) for the suggestion!

[Submit your suggestions and votes for next week][submit_crate]!

[submit_crate]: https://users.rust-lang.org/t/crate-of-the-week/2704

# Call for Participation

Always wanted to contribute to open-source projects but didn't know where to start?
Every week we highlight some tasks from the Rust community for you to pick and get started!

Some of these tasks may also have mentors available, visit the task page for more information.

* [Call for Maintainers - criterion-plot](https://users.rust-lang.org/t/call-for-maintainers-criterion-plot/24413).

If you are a Rust project owner and are looking for contributors, please submit tasks [here][guidelines].

[guidelines]: https://users.rust-lang.org/t/twir-call-for-participation/4821

# Updates from Rust Core

186 pull requests were [merged in the last week][merged]

[merged]: https://github.com/search?q=is%3Apr+org%3Arust-lang+is%3Amerged+merged%3A2019-01-21..2019-01-28

* [enable RISC-V atomic compare and swap](https://github.com/rust-lang/rust/pull/57925)
* [recover from parse errors in literal struct fields and incorrect float literals](https://github.com/rust-lang/rust/pull/57779)
* [merge visitors in AST validation](https://github.com/rust-lang/rust/pull/57730)
* [resolve: Fix span arithmetics in the import conflict error](https://github.com/rust-lang/rust/pull/57908)
* [fix race condition when emitting stored diagnostics](https://github.com/rust-lang/rust/pull/57066)
* [don't ICE when logging unusual types](https://github.com/rust-lang/rust/pull/57865)
* [combine all builtin early lints](https://github.com/rust-lang/rust/pull/57726)
* [add suggestion for moving type declaration before associated type bindings in generic arguments](https://github.com/rust-lang/rust/pull/57886)
* [add suggestion for incorrect field syntax](https://github.com/rust-lang/rust/pull/57863)
* [suggest removing leading left angle brackets](https://github.com/rust-lang/rust/pull/57852)
* [add error for trailing angle brackets](https://github.com/rust-lang/rust/pull/57817)
* [print visible name for types as well as modules](https://github.com/rust-lang/rust/pull/57802)
* [use structured suggestion instead of notes](https://github.com/rust-lang/rust/pull/57795)
* [explain type mismatch cause pointing to return type when it is `impl Trait`](https://github.com/rust-lang/rust/pull/57793)
* [when using value after move, point at span of local](https://github.com/rust-lang/rust/pull/57294)
* [conditionally skip two passes if their related attributes were not found](https://github.com/rust-lang/rust/pull/57691)
* [fix evaluating trivial drop glue in constants](https://github.com/rust-lang/rust/pull/57734)
* [const_eval: predetermine the layout of all locals when pushing a stack frame](https://github.com/rust-lang/rust/pull/57677)
* [fix memory leak in `P::filter_map`](https://github.com/rust-lang/rust/pull/57667)
* [get rid of the fake stack frame for reading from constants](https://github.com/rust-lang/rust/pull/57606)
* [add intrinsic to create an integer bitmask from a vector mask](https://github.com/rust-lang/rust/pull/57269)
* [un-deprecate `mem::zeroed`](https://github.com/rust-lang/rust/pull/57825)
* [make `MutexGuard`'s `Debug` implementation more useful](https://github.com/rust-lang/rust/pull/57703)
* [make `str` indexing generic on `SliceIndex`](https://github.com/rust-lang/rust/pull/57604)
* [small perf improvement for `fmt`](https://github.com/rust-lang/rust/pull/57537)
* [add signed `num::NonZeroI*` types](https://github.com/rust-lang/rust/pull/57475)
* [std: stabilize fixed-width integer atomics](https://github.com/rust-lang/rust/pull/57425)
* [use pinning for generators to make trait safe](https://github.com/rust-lang/rust/pull/55704)
* [implement `optimize(size)` and `optimize(speed)` attributes](https://github.com/rust-lang/rust/pull/55641)
* [cargo: make incremental compilation the default for all profiles](https://github.com/rust-lang/cargo/pull/6564)
* [rustdoc: fix ICE from loading proc-macro stubs](https://github.com/rust-lang/rust/pull/57846)

## Approved RFCs

Changes to Rust follow the Rust [RFC (request for comments)
process](https://github.com/rust-lang/rfcs#rust-rfcs). These
are the RFCs that were approved for implementation this week:

* [RFC 2235: Implement Debug, Eq, PartialEq, and Hash for libc structs](https://github.com/rust-lang/rfcs/pull/2235).

## Final Comment Period

Every week [the team](https://www.rust-lang.org/team.html) announces the
'final comment period' for RFCs and key PRs which are reaching a
decision. Express your opinions now.

### [RFCs](https://github.com/rust-lang/rfcs/labels/final-comment-period)

* [disposition: postpone] [impl trait expressions](https://github.com/rust-lang/rfcs/pull/2604).
* [disposition: postpone] [Direct and Partial Initialization using &uninit T](https://github.com/rust-lang/rfcs/pull/2534).
* [disposition: close] [Item-level blocks (was: Item-level *scopes*)](https://github.com/rust-lang/rfcs/pull/2377).

### [Tracking Issues & PRs](https://github.com/rust-lang/rust/labels/final-comment-period)

* [disposition: merge] [Stabilize extern_crate_self](https://github.com/rust-lang/rust/pull/57407).

## New RFCs

* [`#[link(kind="dll")]`](https://github.com/rust-lang/rfcs/pull/2627).

# Upcoming Events

### Online

* [Jan 30. Rust Events Team Meeting on Telegram](https://t.me/joinchat/EkKINhHCgZ9llzvPidOssA).
* [Feb  6. Rust Community Team Meeting on Discord](https://discordapp.com/channels/442252698964721669/443773747350994945).

### Africa

* [Feb  6. Sandown, ZA - Johannesburg meetup](https://www.meetup.com/Johannesburg-Rust-Meetup/events/qbhxmqyzdbjb/).

### Europe

* [Jan 24. Hamburg, DE - Rust Hack & Learn Hamburg](https://www.meetup.com/Rust-Meetup-Hamburg/events/257153030/).
* [Jan 30. Toulouse, FR - Rust Toulouse](https://www.meetup.com/fr-FR/Toulouse-Rust-Meetup/events/257926837/).
* [Jan 31. Helsinki, FI - Helsinki Rust meetup](https://www.meetup.com/Finland-Rust-Meetup/events/257863678/).
* [Jan 31. Torino, IT - Turin Rust meetup](https://www.meetup.com/Mozilla-Torino/events/sbtclqyzcbgc/).
* [Feb  3. Bruxelles, BE - Rust Dev Room @ FOSDEM](https://fosdem.org/2019/).
* [Feb  6. Berlin, DE - Berlin Rust Hack and Learn](https://www.meetup.com/opentechschool-berlin/events/rjgkhqyzdbjb/).
* [Apr 26-29. Berlin, DE - OxidizeConf tickets are now available](https://oxidizeconf.com/).

### North America

* [Jan 28. Durham, US - Triangle Rustaceans](https://www.meetup.com/triangle-rustaceans/).
* [Jan 30. Chicago, US - Chicago Rust Meetup - Property-Based Testing in Rust](https://www.meetup.com/Chicago-Rust-Meetup/events/257469240/).
* [Jan 31. Phoenix, US - Phoenix Rust: Games](https://www.meetup.com/Desert-Rustaceans/events/257976456/).

If you are running a Rust event please add it to the [calendar] to get
it mentioned here. Please remember to add a link to the event too.
Email the [Rust Community Team][community] for access.

[calendar]: https://www.google.com/calendar/embed?src=apd9vmbc22egenmtu5l6c5jbfc%40group.calendar.google.com
[community]: mailto:community-team@rust-lang.org

# Rust Jobs

* [Rust Engineer at slowtec Stuttgart, DE](https://www.reddit.com/r/rust/comments/ahahqj/job_rust_engineer_position_in_stuttgart_de/).

*Tweet us at [@ThisWeekInRust](https://twitter.com/ThisWeekInRust) to get your job offers listed here!*

# Quote of the Week

> Rust is kind of nice in that it lets you choose between type erasure and monomorphization, or between heap-allocation and stack-allocation, but the downside is that you have to choose.

– Brook Heisler [on discord](https://discordapp.com/channels/442252698964721669/448238009733742612/536406836178583562) (login needed, sorry!)

Thanks to [scottmcm](https://users.rust-lang.org/t/twir-quote-of-the-week/328/614) for the suggestion!

[Please submit your quotes for next week](http://users.rust-lang.org/t/twir-quote-of-the-week/328)!

*This Week in Rust is edited by: [nasa42](https://github.com/nasa42), [llogiq](https://github.com/llogiq), and [Flavsditz](https://github.com/Flavsditz).*

<small>[Discuss on r/rust]().</small>