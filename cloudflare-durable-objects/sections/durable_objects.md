# Durable objects 🪨

### to the rescue

---

## What are durable objects?

---

<img class="r-stretch" src="./assets/durable_objects_are_workers.png" />

---

## What are durable objects?

* Built on top of workers
* Built in persistence (K/V store, SQLite) <!-- .element: class="fragment" data-fragment-index="2" -->
* Each instance (ID) <!-- .element: class="fragment" data-fragment-index="3" -->
  * Single-threaded
  * Data co-located with application
  * Owns its state
* Written in JavaScript or WASM <!-- .element: class="fragment" data-fragment-index="4" -->

---

<img class="r-stretch" src="./assets/workers_3.png" />

---

<img class="r-stretch" src="./assets/durable_objects_1.png" />

---

<img class="r-stretch" src="./assets/durable_objects_2.png" />

---

# Demo!

#### Again 🎉

---

## Other features

* Websockets <!-- .element: class="fragment" data-fragment-index="1" -->
* Wake up alarms <!-- .element: class="fragment" data-fragment-index="2" -->
* RPC from workers <!-- .element: class="fragment" data-fragment-index="3" -->
* SQLite (with PITR) since September <!-- .element: class="fragment" data-fragment-index="4" -->

---

## Use cases

* Real time collaboration
* Booking systems
* CI/CD pipelines
* Doom <!-- .element: class="fragment" data-fragment-index="1" --> ([play](https://silentspacemarine.com/)) <!-- .element: class="fragment" data-fragment-index="1" -->
