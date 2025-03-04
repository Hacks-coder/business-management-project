<script lang="ts">
  import { Accordion, AccordionItem } from "svelte-accessible-accordion";
	import Small from "../Texts/Small.svelte";
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

<section class="@container">
    <div class="text-xl font-bold flex gap-5 flex-col items-center mt-30 @4xl:flex-row @4xl:justify-center">
        <div>
            <img src="/others/faqs.png" alt="" class="size-72 @xl:size-100 @3xl:size-120">
        </div>
        <Accordion>
            {#each faqs as {question, answer}}
                <AccordionItem title= {question} class="shadow-sm shadow-gray-300 p-2 w-80 @md:w-100 @xl:w-120 @4xl:w-150">
                    <Small text = {answer} className = "text-sm" />
                </AccordionItem>
            {/each}
        </Accordion>
    </div>
</section>