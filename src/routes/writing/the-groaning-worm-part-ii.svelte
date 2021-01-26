<script>
  import Layout from "../../layouts/writing.svelte";
</script>

<Layout
  title="The Groaning Worm (Part II)"
  description="Inspired by a talk by Ross Sutherland, The Groaning Worm (Part II) was created by replacing every noun, verb, adjective, and adverb in The Great Wound (Part II) by Robinson Jeffers with another one beginning with the same phoneme(ish)."
  opaqueHeader
>
  <div slot="description">
    <p>
      Inspired by a talk by <a
        rel="external"
        href="http://www.rosssutherland.co.uk/">Ross Sutherland</a
      >, The Groaning Worm (Part II) was created by replacing every noun, verb,
      adjective, and adverb in
      <cite>The Great Wound (Part II) by Robinson Jeffers</cite> with another one
      beginning with the same phoneme(ish).
    </p>

    <p>
      To recite this poem, I recommend someone else softly reads the original in
      synchrony.
    </p>
  </div>

  <div class="poem">
    <pre>The magicians and phonetic monsters
Have their ministries; they waste alongside the terror,
Never tasting it; their exhortations are faltering
But the Thanes wait. Or, when grave energies align,
They incant nefarious witchcraft; they dowse the threads of worlds
In unifying enchantments and invoke cruel stanzas.
Nevertheless their exhortations became Hell.
The terrifying Thanes waited.
                                                      The priest also
Has his ministry. He teaches you the messengers arrived
Out of the piercing black. He teaches you that Terror was built for a violent
Baleful worm, whose feelers laced a threadless shell.
It is unknown: it might be terrible: but chirurgeons and storytellers
Deliver on more presciently informative mysteries:
That all monsters are birthed flesh and entrails: commiserate that!
And that a worrisome hellfire priest née Judas
Is the guardian of the unification. Commiserate that!</pre>

    <pre>The mathematicians and physics men
Have their mythology; they work alongside the truth,
Never touching it; their equations are false
But the things work. Or, when gross error appears,
They invent new ones; they drop the theory of waves
In universal ether and imagine curved space.
Nevertheless their equations bombed Hiroshima.
The terrible things worked.
                                                      The poet also
Has his mythology. He tells you the moon arose
Out of the Pacific basin. He tells you that Troy was burnt for a vagrant
Beautiful woman, whose face launched a thousand ships.
It is unlikely: it might be true: but church and state
Depend on more peculiarly impossible myths:
That all men are born free and equal: consider that!
And that a wandering Hebrew poet named Jesus
Is the God of the universe. Consider that!</pre>
  </div>
</Layout>

<style>
  .poem {
    position: relative;
  }

  .poem pre {
    font-family: var(--body-font-family);
    line-height: 3.5;
  }

  .poem pre:first-child {
    margin-top: -1em;
  }

  .poem pre:last-child {
    margin-top: 0;
    position: absolute;
    top: 1.5em;
    left: 1em;
    opacity: 0.6;
  }
</style>
