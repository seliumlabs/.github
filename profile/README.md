# Selium

Selium is an extremely developer friendly composable messaging platform with zero build time
configuration.

## Features

#### Developer-first, but for real

Selium is trivial to setup and feels instantly familiar on implementation. Selium's client library
implements [Tokio](https://tokio.rs)'s `Stream` and `Sink` traits, so chances are you already know
how to use it.

#### Zero build time config

Yep! Unlike other platforms where pipelines have to be established ahead of time using a GUI or
CLI, Selium builds and runs pipelines on the fly. With Selium you can throw away your continuous
deployment and get on with coding.

| :nerd_face: Nerd Alert!                                                                                                             |
| ----------------------------------------------------------------------------------------------------------------------------------- |
| Internally we use a lock-free double-ended tree to manage clients and their various requirements. This graph drives all of our I/O. |

#### Messaging patterns

Selium supports both publish-subscribe and RPC patterns, allowing you to disseminate data and
consume services over the same platform. No more gagging while you reach for that REST toolkit!

#### Namespaces FTW!

Selium uses namespaces to achieve segmentation between facets of your data network. You can
arbitrarily define namespaces much the same way as you'd create directories in a filesystem. Selium
enforces isolation between namespaces at the user level (see mTLS), so sharing between namespaces
is simple, but secure.

#### QUIC protocol

On the wire, Selium uses the [QUIC protocol](https://quicwg.org). QUIC is a UDP-based successor to
TCP and is designed to address many of TCP's shortcomings. Unlike raw UDP, QUIC is robust and
reliable, so much so that HTTP/3 is built atop it!

We also like QUIC because it natively supports encrypted transport, which is a perfect segue to...

#### Security

Selium is written in Rust, which, for the uninitiated, eliminates an entire class of
memory-based vulnerabilities.

Selium also supports mTLS out of the box for securing client-server communication in both
directions.

#### But wait, there's more!

There's too much to say in such a small space, so here's some stuff we missed out, rapid fire!
- Map, filter, split and join your streams (coming soon)
- Message retention, replay and delivery guarantees (coming soon)
- Embedded WASM support (coming soon)
- Granular ACLs (coming soon)
- Some secret stuff that we can't wait to tell you about. We're not good at keeping secrets!

## Getting started

Check out [seliumlabs/selium](https://github.com/seliumlabs/selium) for more info.

## Stay in the know

[Sign up to our mailing list](https://selium.com/#signup) to stay across the latest updates.
