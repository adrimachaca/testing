<template>
   <div class="task-container">
      <div class="task-dept">
         <p>Department</p>
      </div>
      <div class="task-body">
         <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent convallis, magna a vulputate porttitor.</p>
      </div>
      <div class="task-footer">
         <button class="edit-btn"><i class="pi pi-pencil" style="font-size: 1rem"></i></button>
         <button class="delete-btn"><i class="pi pi-trash" style="font-size: 1rem"></i></button>
      </div>
   </div>
</template>

<style scoped>
   .task-container {
      margin-top: 20px;
      padding: 15px;
      border-radius: 8px;
      box-shadow: 0px 0px 5px 0px rgba(0,0,0,0.15);
      display: flex;
      flex-direction: column;
   }

   .task-dept {
      padding-bottom: 5px;
      margin-bottom: 10px;
   }
   .task-dept p {
      font-size: 0.8rem;
      color: #686D76;
   }

   .task-body {
      margin-bottom: 10px;
   }

   .task-footer {
      display: flex;
      flex-direction: row;
      justify-content: flex-end;
      margin-top: 10px;
   }

   .task-footer button {
      border: none;
      margin-left: 15px;
      padding: 8px 10px;
      cursor: pointer;
   }

   .edit-btn {
      color: #686D76;
      background-color: #E0E0E0;
      border-radius: 7px;
   }

   .delete-btn {
      color: #FF6969;
      background-color: #FFD4E0;
      border-radius: 7px;
   }
</style>