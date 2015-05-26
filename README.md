# Logla Case

This project is a variation of the Logla language that uses a case tag argument system instead of ordinal arguments.

While it would be ideal if this system could be purely an isolated extension to the orginal language (and on purely techincal grounds that is possible) doing so would limit the capability of the case system, not allowing it to reach its full potential. A clear example of this limitation can be seen in the Lojban words `bajra` and `bajykla`. In Lojban, `bajra` means `x1 runs on x2 using limbs x3 with gait x4`. To convey the idea of moving to and fro while running, it must provide the compound word `bajykal`, which combines `bajra` with the word for go/come, `klama`. With a case tag system this would not be necessary -- `bajra` would sufficent in itself supporting to and fro arguments, as well as any others that are pertenant to the concpet of running.

## What are Case Tags?

Case Tags are words that name the argument slots of predicates. By giving the argument slots these *tags*, they can be referenced without dependence on their ordinal positions. Tags are the vocalic forms of root words and thus can vary greatly to garner any necessary meaning. But if all tags were so unique it would largely defeat their usefulness. Rather, predicates typically draw from a common pool tags and assign them according to similarity of role. These roles are the cases, hence the term *case tag*.

Predicates can be grouped according to the tags they support. Each group represents an *archetypal predicate*. All predicates belong to an archetype. If you know the archetype of a word than you also know its case tags. (But not necessarily the order of those tags!)

In addition to a word's specific archetype, all words share a common pseudo-archetype, called the *ordinal archetype*. This archetype simply assigns a number to the arguments of a predicate. In Lojban these are named `fa fe fi fo fu`.

Natural languages typically use prepositions as case tags and tend to lump multiple cases into the connotations of the same words. Words like the English "by" can have many different meanings dependent wholly on context -- "created *by* me", "worked *by* the book", "came *by* the thousands", etc.

Case tags are similar to *types* in programming languages. When a predicate is defined, it's arguments are said to have a *type interface*, specifying which cases are allowed in a given slot.

## An Excursion into Prior Art

### Loglan's Optional Case Tags

Loglan has a set of case tags, largely patterned after natural language.

| Logla' | Loglan | Lojban | English  | Meaning                                        |
|--------|--------|--------|----------|------------------------------------------------|
|        | beu    |        | in       | Patients, Parts, Properties                    |
|        | cau    |        | by,for   | Quantities, Amounts, Values                    |
|        | dio    |        | to,for   | Recipients, Beneficiaries, Destinations        |
|        | foa    |        | in,of    | Wholes, Sets, Collectivities                   |
|        | goa    |        | than     | Greaters in greater/lesser than relations      |
|        | jui    |        | than     | Lessers in greater/lesser than relations       |
|        | kao    |        | by       | Actors, Agents, Doers                          |
|        | neu    |        | under    | Conditions, Fields, Circumstances              |
|        | pou    |        |          | Products, Outputs, Purposes                    |
|        | sau    |        | from     | Start, Sources, Origins, Reasons, Causes       |
|        | veu    |        | by,via   | Events, States, Deeds, Means, Routes, Effects  |

Even with such a small set, or rather, because it is such a small set, debates still arise as to which tags are appropriate for which arguments. Logla' seeks to remedy this by providing a large and more refined set of cases. Logla avoids tag *overload*, placing similar but distinct cases under one label.

### Lojban's Modal Tags

Lojban has *Modal Tags*. As it turns out this is a rather confused mismash of actual case tags and a select set of predicates, simplified and converted to structure words for convenience of speech. Grammatically, they are used as if they were case tags, but in fact they are not. Most of these modal tags are the BAI selma'o listed in Chapter 9, Section 17 of the CLL.

After careful consideration, I have realized that most of Lojban's modal tags are not case tags. Rather they are a short-hand for abstract predicates -- a way to more concisely add a secondary fact to a sentence. For example, `sepu'a` in-order-to-please, is just a way to say `se pluka` on an event abstraction of the rest of a sentence.

Consequently I have realized there are far fewer case tags then I realized. Still considerably more then Loglan's mere eleven -- we can be more precise than that, but nothing in the range of the hundred or two that I expected. Now I expect there will be no more than a few dozen. That might seem like a good thing, but it has a serious downside in that the semantic space is far less utilized. The same case tags will be repeated frequently, only out-done by the reiterations of `le` and `lo`.

I want to given an example, just to be clear about what I mean. Take the word `kam` as the root for `come/go`, than `kamdio` can mean place-that-is-gone-to. That makes perfect sense because `dio` is the tag of the first argument of `kam`. However, if one said `kamni'a`, literally `go down`, one might think that means place-below-that-is -gone-*to*. But it does not, because no where in that word is the idea of *to* actually mentioned. It could just as well be *from*, or *via*. In other words, strictly as given, it is non-nonsensical.

On the other hand, perhaps there is an opportunity here to solve the following issue with the grammar. Because the case tags when used to mark off a sumit are the same as the tags appended to root words, it can at times be a little daunting to decipher what is being said.

    mi kam-cu dio bajkam-dio ti.
    I go to the-place-run-to from here.

Notice the two uses of `dio`. While technically correct, one can see how a slight mishearing could lead one to think `mi kam-cu dio ti` -- I was coming here. If there were perhaps some additional dimension applicable to end-tags, e.g. `dia` and `diu` as meaningful variants of `dio`, then this (albeit minor) issue would be moot as would the issue of a such a limited set of case tags. That's kind of putting the cart before the horse, but it's worth consideration.

## Derivation of Tags from Roots

**NOTE: How this works is still to be determined. See [[Vocalic Forms]] for a review of some of the possibilities. The following presents the simplest of them.**

Unlike Loglan or Lojban, the djifoa/rafsi serve more purposes than simply components of lujvo/ , they also can serve as the basis of case tags. 

Any root can be transformed into it's *vocalic form* through a simple procedure of converting the last constant into a vowel and adding `'`.

    CCV  ->  CV'V (CCV can be used for case endings but not predicate tags) 
    CVC  ->  CV'V

If the CVC or CVC/CCVC root proposal is adopted (see [[]]) then,

    CVC  ->  CV'V or CCV (if diphthong is permissible)
    CCVC ->  CCV'V

There are of course too few `CV'V` forms to have a one-to-one correspondence with every consonant. This turns out not to be as problematic as it might first appear because of the similarity of certain constants which tend to steer the root words themselves away from these overlaps. The following translation table should make this clear.

| Consonant  | Vocalic Transform |
|------------|-------------------|
| b,p,m      | 'o                |
| t,d,n      | 'e                |
| k,g,x,r    | 'a                |
| f,v        | 'u                |
| s,z,c,j,l  | 'i                |

On average, each root shares a vocalic form with about three other roots.

In addition, common tags, because they are common, are given an abbreviated form of just `CV`, dropping the ending `'V`. This frees up the `CV'V` to be more uniquely associate with the other roots that fit the derivation. Because common case tags are used far more often than not, in the end, there are actually very few overlaps of any significance, and these can simply be noted as part of words *etymology*.

## Common Case Tags

Logla Prime's case tags are derived bottom-up from usage rather then all forced into a theoretical top-down schema. Technically a predicate could have case tags no other predicate shares. However in practice it is much more useful if there are common tags for similar roles. These *common tags* are determined by looking for similar argument patterns between predicates and establishing [[Predicate Archetypes]].

(Note: The words presently given for each term are primarily from Lojban. That will change!)

| Vowelic  | Root    | Role                    | Notes                      |
|----------|---------|-------------------------|----------------------------|
|          |         | Identity                |                            |
| sa       | sat     | Origin                  | mam, prim ?                |
|          |         | Destination             |                            |
| ke       | ken     | Patient                 |                            |
| fa       | far     | Agent                   |                            |
|          |         | Agent + Patient         |                            |
| sfa      | satfar  | Agent + Origin          |                            |
|          |         | Agent + Destination     |                            |
|          |         |                         |                            |
| sepa'u   |         | Composition             |                            |
|          |         |                         |                            |
| sema'e   |         | Material Composition    |                            |
| sepi'o   |         | Instrument              |                            |
|          |         | Purpose, Goal           |                            |
|          |         | Circumstance            |                            |
| ja'e     |         | Result                  |                            |
| mai      | maj     | Greater                 | or ak or kab ?             |
| mei      | men     | Lesser                  |                            |
| ke'e     | ek      | Equal                   |                            |



* **Nominal** Simple reference by name. If no other tag seems to fit, this is probably the tag you want. (e.g. The **cat** is calico.)

* **Agent** The causal agent of an action. (e.g. **He** does.)

* **Patient** The medium of change. (e.g. He gives **it** to me.)

* **Patient + Agent** The causal agent that is also the patient. (e.g. **He** jumps.)

* **Origin** The source of the patient. (e.g. He came from the **store**.)

* **Origin + Agent** The causal agent that is also the origin. e.g. **He** gives.

* **Destination** The destination (e.g. He gives it to **me**.)

* **Destination + Agent** The causal agent that is also the destination. (**He** takes.)

* **Identity** Symmetrical identity, can be used multiple times in a single predication. (**He** is the **crook**).

* **Referent** The object of reference in a link, or non-quantitative comparison. (e.g. Dogs are similar to **wolves**.)

* **Target** The target object of a link or non-quantitative comparison. (e.g. **Dogs** are similar to wolves.)

* **Quality** State of being or property. (e.g. I feel **great**.)

* **Greater** The greater of a quantitative comparison. (e.g. **This** weighs more than that.)

* **Lesser**  The lesser of a quantitative comparison. (e.g. This weighs more than **that**.)

* **Standard** The standard of a comparison. (e.g. ?)

* **Quantity** The degree, level, quantity or amount. (e.g. It costs a **dollar**).

* **Whole** (e.g. The cub is a member of the **pride**.)

* **Component** Constituent part of a whole. (e.g. The **cub** is a member of the pride.)

* **Material** Subset of Component but limited to material make-up. (e.g. It is made entirely out of **wood**.)

* **Instrument** (e.g. He hit it with his **hand**.)

* **Method** Similar to instrument but describes a technique or procedure of an action. (e.g. He fixed it with the **instructions**.)

* **Circumstance** (e.g. He did it because of the **heat**.)

* **Result** The actualized consequences or effects of an action. (e.g. He molded it into a **house**.)

* **Purpose** The intended consequences or effects of action. (e.g. He did it to **win**.)

* **Location** Subset of ... limited to space. (He stayed **here**.)

* **Location + Origin** Subset of Origin limited to space. (e.g. He came from the **store**.)

* **Location + Destination** Subset of destination limited to space. (e.g. He went **home**.)

* **Route** (e.g. He traveled via the **road**.)

* **Time** Subset of ... limited to a instance of time. (e.g. We  **early**.)

* **Time + Origin** Subset of origin limited to time (e.g. We begin in the **morning**.)

* **Time + Destination** Subset of destination limited to time. (e.g. He arrived a **dawn**.)

* **Form** - Form, type or classification. (e.g. File it under **unicorns**.)

* **Manner** (*u.a.*) Similar to method, but ... (e.g. He ran **hard**.)

* **Possessor** (e.g. **He** owns the **car**.)

* **Possession** (e.g. He owns the **car**.)

* **Action** Subclass of Nominal limited to an an event or deed. Rarely used, since Nominal usually works.



## New Grammar

Simple formula

    rafsi/djifoa + case-tag = "gismu"

This process is called nominalization. A root cannot be used until it is nominalized. (There a few places where it might possible, but for consitancy it might better to make it altogether illegal.) The essential effect of nominalization is to reduce a predicate to a one argument nominal form.

Besides relational predicates (predicts with more than one argument) the Logla vocabulary can have *free nominals*. Free nominals are non-relational predicates (having only one argument) whose case is not tied to the meaning of the root. Lets look at an example.

  rut - x1 (na) is a fruit of species x2 (ju'e)
  ric - x1 (na) is a tree of species x2 (ju'e)

  rutri'i = fruit tree

Notice that ri'i is the vocalic translation of ric, but ri'i is not a case of rut -- only `na` and `ju'e` are. So this word is a free nominal and cannot be used as a predicate other than to say "X is a fruit tree".

Since case tags derive from root words, a speaker can be redundant by using a root and it's derived tag together. For example, in Lojban `gau` is derived from `gasnu`. In Logla' let us assume the root is `gas`, then `gas gau` would be a rather redundant way to say "doer", literally "the doer of doing".

Since the small words and case tags share the same morphology, namely CV and CV'V, they must adhere to strict set of grammar rules so they are never mistaken for one another.

As case-endings, the case-tags are fairly easy to recognize. They always follow a `CVC` or `CCVC` form.

As predicate place tags, the case-tags must immediately follow the a clause dividing structure word. But they are optional (without them the order of clauses specify case). This can make the tags a little more difficult to immediately identify. But since any predicate only has a finite number of cases, knowing the predicate make's it much easier to identify them. (Note, `le` will probably have to change, but we leave it for now.)

    mi kamcu le fe rutri'i le fa zdani mi
    I come from the fruit tree to my home.

Notice the use of `fe` and `fa`. These are the ordinal case tags, and we have used them in this example to switch the normal places of "to" and "from". Notice also that they fall right after `le`, the structure word that serves to break the sentence into clauses. (Also, notice that `mi` comes after `zdani`. This is because in Logla, unlike Lojban and Loglan, modifiers run to the right, the to the left.)


I have been trying to work out a modified grammar that works in case tags, both in identifying the arguments of the selbri and the internal positions of the sumti. It is not proving easy.

    mi kam cu la run fe la spein.
    I come/go to the running destination from Spain.

Notice that if we change `fe` to the case tag `dio` ambiguity ensues.

    mi kam cu la run dio la spein.

Technically it is still decipherable, but just barely. It only works if the end-tags are mandatory. If we all the other tags we can see why more easily.

    kao mi kam cu dio la run dio sau la spein.

It may suffice, but it gets worse trying to complete more information about `la run`. A complete relative clause does the trick,

    kao mi kam cu dio la run poi dio ke'a sau lo pak ko'u sau la spein.

But using the Loglan je/jue short-cuts gets even hairier. Should the clause go between `run` and `dio` or after `dio`?

    kao mi kam cu dio le run je sau le pak fa dio sau la spein.
    kao mi kam cu dio le run dio je sau le pak fa sau la spein.

It would seem that the second it would have to be the first least the second `dio` be thought an additional term in the relative clause. 

    kao mi kam cu dio le run dio je sau le pak fa sau la spein.

It's not as bad to *see* if the end-tags are join with the word they modify.

    kao mi kam cu dio le rundio je sau le pakfa sau la spein.


## Tag Modifiers, The New Modals

Note that if a word has a `-` before or after it is intended to be used as a prefix or suffix on related words, but it can still be used alone.


### Existential

### Agent Modifiers

| Logla' | Meaning                                     |
|--------|---------------------------------------------|
| gau    | Intentional               |
|        | Indirect (Instigator)     |
|        | Incidental/Unintentional  |

### Spacial Modifiers

Spacial modifiers can be used on any *locative* case. They can also be
used alone, in which case they imply *nominal locative*. 

| Logla' | Meaning                                   |
|--------|-------------------------------------------|
| ga'u   | Above                                     |
| ni'a   | Below                                     | 
| ca'u   | Front, Bow                                |
|        | Behind, Aft                               |
| zu'a   | Left, Starboard                           |
| ri'u   | Right, Portside                           |
| ne'i   | Inside, Within                            |
|        | Outside                                   |
|        | In Contact, Touching                      |
|        | Near                                      |
|        | Within Range                              |
|        | Out of Range                              |
| be'a   | North                                     |
|        | West                                      |
|        | East                                      |
|        | South                                     |

### Temporal Modifiers

| Logla' | Meaning                                   |
|--------|-------------------------------------------|
| pu     | Before                                    |
| ba     | After                                     |

### Degree Modifiers

Degree modifiers apply to other modifiers.

| Logla'    | Meaning                      |
|-----------|------------------------------|
|           | Infinitesimal, Touching      |
| -vi, -zi  | Small, Near                  |
| -va, -za  | Medium, Midway               |
| -vu, -zu  | Large, Far                   |
|           | Vast, Unreachable            |
|           | Least, Worst                 |
|           | Most, Best                   |



## Common Lujvo Roots

| Logla' | Loglan | Lojban | Meaning                                   |
|--------|--------|--------|-------------------------------------------|
|        | pua    |        | Word, Grammatical term                    |
|        |        |        | Nature, Essence  (e.g. childhood)         |
|        |        |        | Spirit                                    |




