<script lang="ts">
  import { Accordion, AccordionItem } from "svelte-accessible-accordion";
	import Small from "../Texts/Small.svelte";
	import Title from "../Texts/Title.svelte";
  const faqs = [
    {
        question: " is there a free trial avaliable?",
        answer: " is there a free trial avaliable?"
    },
    {
        question: " is there a free trial avaliable?",
        answer: " is there a free trial avaliable?"
    },
    {
        question: " is there a free trial avaliable?",
        answer: " is there a free trial avaliable?"
    },
    {
        question: " is there a free trial avaliable?",
        answer: " is there a free trial avaliable?"
    },
  ]
</script>

<section class="text-xl font-bold flex gap-5 flex-col items-center mt-30">
    <div>
        <img src="/others/faqs.png" alt="">
    </div>
    <Accordion>
        {#each faqs as {question, answer}}
            <AccordionItem title= {question} class="shadow-sm shadow-gray-300 p-2 w-80">
                <Small text = {answer} className = "text-sm" />
            </AccordionItem>
        {/each}
    </Accordion>
</section>