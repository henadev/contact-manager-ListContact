<template>
<ul class="list-group"> 
    <li class="list-group-item" v-for="contact  in contactsList" :key="contact.id" @mouseover="$emit('mouse-over-contact', contact)">
        {{contact.name}}
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