[FR](./LISEZMOI.md)
[ES](./LEERME.md)

# Peer-to-Peer web apps: a Disruptive Kata

## Internet is decentralized... why should we care about peer-to-peer?

Internet original design and its common applicaitons make use a client-server
architecture. That's not a coincidence since `http` protocol is tinted with
this paradigm.

It is not incompatible with the decentralized network architecture of internet
simply because... internet do not have only one server! Hence, web clients
(usually a browser) can establish connections with many servers. Moreover,
servers can communicate between themself. And servers can be redundant, that is
to say that many can deliver the same information. And their can be more than
one route from a client to the server.

This decentralised design foreshaodwed that anyone could take part to
the network and publish its own content. And we generally consider that it is
the case.

But how to achieve it when you do not control a server publicly acessible from
the internet?

![xkcd: the file transfer problematic](https://imgs.xkcd.com/comics/file_transfer.png)

We see that despite its decentralized design, the client-server dominant
paradigm have consequenses on our capablility to equally share our data. And,
its not quite difficult to find drawbacks of asking to a third party to
publish it or to transact it ou our behalf.

## What is interesting in this kata?

In this kata, we will find ways to establish a direct peer-to-peer communication
between two web client applications.

Also, we will explore the limits of this approach imposed by the actual design
of internet. And we'll ways to get around them.

## Prototypical application

This section describe the general requirements of a web client peer-to-peer
applicaiton:

  - Two web clients or more want to communicate together without the need of
    a third party.
  - The web clients are not obliged to be connected to internet,
    they can be connected to:
      - the same local network,
      - two different network able to esblish a connection between them,
      - no network at all.
  - The web clients do not:
    - a permanent or fiexed ip address or
    - a url allowing one to find its ip address.
  - The web clients can find each other.
  - The web clients can establish a connection.
  - It would be advisable that the web clients validate the users identity.
  - And then, web clients exchange information of value to the users.
