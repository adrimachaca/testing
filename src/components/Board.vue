<template>
   <div class="board">
      <div class="status-col">
         <div class="header-status">
            <h3 class="pill-todo">Todo</h3>
         </div>
      </div>
      <div class="status-col">
         <div class="header-status">
            <h3 class="pill-inprogress">In Progress</h3>
         </div>
      </div>
      <div class="status-col">
         <div class="header-status">
            <h3 class="pill-done">Done</h3>
         </div>
      </div>
   </div>
</template>

<style scoped>
   .board {
      background-color: #fff;
      width: 100%;
      height: 100%;
      padding: 10px;
      margin-left: 20px;
      border-radius: 10px;
      display: flex;
      flex-direction: row;
      box-shadow: 0px 2px 10px 0px rgba(0,0,0,0.1);
   }

   .status-col {
      width: 33.33%;
      padding: 20px;
      margin: 10px;
      box-shadow: 0px 0px 5px 0px rgba(0,0,0,0.15);
      border-radius: 8px;
   }

   .header-status {
      border-bottom: 1px solid #e0e0e0;
      padding-bottom: 20px;
      display: flex;
      flex-direction: column;
      align-items: flex-start;
   }

   .pill-todo {
      padding: 8px 20px;
      background-color: #ffd4e0;
      border-radius: 7px;
   }

   .pill-inprogress {
      padding: 8px 20px;
      background-color: #ffeab6;
      border-radius: 7px;
   }

   .pill-done {
      padding: 8px 20px;
      background-color: #cff5d1;
      border-radius: 7px;
   }
</style>