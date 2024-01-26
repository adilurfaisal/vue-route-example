<template>
    <div>
      <b>Test 2 </b> {{ date }}
    </div>
  </template>

  <script>
  module.exports = {
    name: "Dashboard",
    data() {
      return {
        date: new Date()
      };
    },
    mounted(){
        setInterval(()=>{
            this.date = new Date();
        }, 500)
    }
  };
  </script>
