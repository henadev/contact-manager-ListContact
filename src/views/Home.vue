<template>
<section class="row">
<div class="col-6">
<ContactList :contactsList="contactsList"  @mouse-over-contact="updateHoveredContact"
      @mouseleave="hoveredContact = null"></ContactList>
</div>
<div class="col-6">
<ContactDetails v-if="hoveredContact !== null" :contact="hoveredContact"></ContactDetails>
</div>
</section>


</template>

<script>

import ContactList from '@/components/ContactList.vue';
import ContactDetails from '@/components/ContactDetails.vue';

export default {
  name: "Home",
    components: { ContactList, ContactDetails },
    methods: {
    updateHoveredContact(contact) {
      this.hoveredContact = contact;
    }
  },
  data() {
    return{
      hoveredContact: null,
      contactsList: [
        {
          id: 1,
          name: "Leanne Graham",
          email: "leanne.graham@gmail.com",
          phone: "+21622334455",
          address: {
          street: "Kulas Light",
          city: "Gwenborough",
          },
        },
        {
          id: 2,
          name: "Ervin Howell",
          email: "Shanna@melissa.tv",
          phone: "010-692-6593 x09125",
          address: {
          street: "Victor Plains",
          city: "Wisokyburgh",
          },
        },
        {
          id: 3,
          name: "Clementine Bauch",
          email: "Nathan@yesenia.net",
          phone: "1-463-123-4447",
          address: {
          street: "Douglas Extension",
          city: "McKenziehaven",
          }
        }
      ],   
    }
  }
};
</script>
