<script lang="ts">
  import LinkButton from "./LinkButton.svelte";

  export let language:number = 0;

  $: displayText = ["Download", "Download lah", "Hā-chái", "Hā-tsái"][language];
</script>

<LinkButton name={displayText} link={"/fonts/Indeciso_2.7.otf"} download={"/fonts/Indeciso_2.7.otf"}>
  <svg width="24" height="24" viewBox="0 0 1000 1000" xmlns="http://www.w3.org/2000/svg" fill="currentColor"><path d="M 225 713C 225 713 775 713 775 713C 789 712 801 719 808 731C 815 743 815 757 808 769C 801 781 789 788 775 788C 775 788 225 788 225 788C 211 788 199 781 192 769C 185 757 185 743 192 731C 199 719 211 712 225 713C 225 713 225 713 225 713M 499 137C 510 137 519 141 527 148C 534 155 538 165 538 175C 538 175 538 534 538 534C 538 534 698 373 698 373C 708 364 722 360 735 363C 748 367 758 377 762 390C 765 403 761 417 752 427C 752 427 530 648 530 648C 523 657 512 663 500 663C 488 663 477 658 470 648C 470 648 248 427 248 427C 238 416 234 400 240 386C 246 371 259 362 275 362C 285 362 294 366 302 373C 302 373 462 534 462 534C 462 534 462 175 462 175C 462 154 479 137 499 137C 499 137 499 137 499 137"/></svg>
</LinkButton>

<style>
  svg{
    width: 50%;
    height: 50%;
  }
</style>