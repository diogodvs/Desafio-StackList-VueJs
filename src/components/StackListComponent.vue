<template>
    <div class="w-[49.56rem] grid grid-cols-3 m-auto bg-black-400 rounded-lg border-[1px] h-44 border-orange-100 text-white-txt ">
        <ul 
        class="leading-8 text-[20px] mx-10 my-1 list-disc list-inside max-h-44 "
        v-for="stack in stacks"
        :key="stack.name"
        >
          <li class="text-white-900 w-[15rem] list-item">{{stack.name}}</li>
        </ul>
    </div>
</template>

<script>
export default{
    data(){
    return{
      stacks : 
      [
        {id:1, name: 'Java'},
        {id:2, name: 'SpringBoot'},
        {id:3, name: 'React'},
        {id:4, name: 'VueJs'},
        {id:5, name: 'Javascript'},
        {id:6, name: 'TypeScript'},
        {id:7, name: 'Tailwind Css'},
        {id:8, name: 'Styled Components'},
        {id:9, name: 'Angular'},
        {id:9, name: 'SQL'},
        {id:9, name: 'Node'},
      ], 
    }
}}
</script>