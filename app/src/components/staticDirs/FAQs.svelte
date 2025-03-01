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

<section class="text-xl font-bold flex justify-center mt-30">
    <Accordion class="shadow-sm shadow-gray-700 p-5 rounded-2xl">
        {#each faqs as {question, answer}}
            <AccordionItem title= {question} class="shadow-sm shadow-gray-300 p-2">
                <Small text = {answer} className = "text-sm" />
            </AccordionItem>
        {/each}
    </Accordion>
</section>