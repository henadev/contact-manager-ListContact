<template>
<ul class="list-group"> 
    <li class="list-group-item" v-for="(list,indice)  in contactsList" :key="list.id" @mouseover="updateContact(indice)">
        {{list.name}}
    </li>
</ul>
</template>

<script>
export default {
  name: "ContactList",
  props: {
    contactsList:  Array
  }
}
</script>