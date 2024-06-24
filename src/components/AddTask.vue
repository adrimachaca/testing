<script>

export default {
   data() {
      return {
         departments: [
            { id: 'alldepartments', title: 'All Departments', icon: 'pi-sitemap' },
            { id: 'artistbookings', title: 'Artist Bookings', icon: 'pi-headphones' },
            { id: 'gastronomy', title: 'Gastronomy', icon: 'pi-shop' },
            { id: 'legalSecurityControl', title: 'Legal, Security & Control', icon: 'pi-shield' },
            { id: 'marketing', title: 'Marketing & Sponsors', icon: 'pi-volume-up' },
            { id: 'ticketing', title: 'Ticketing and Pre-sale ', icon: 'pi-receipt' },
            { id: 'stageEquipment', title: 'Stage & Equipment', icon: 'pi-sliders-v' }
         ]
      };
   },

};

</script>
<template>
   <div class="addtask-container">
      <div class="addtask-text">
         <div class="add-title">
            <p>Add new task</p>
         </div>
         <select>
            <option value="" disabled selected>Select department</option>
            <option v-for="department in departments" :value="department.id">{{ department.title }}</option>
         </select>
         <input type="text" placeholder="Write here your task..." />
         <input type="submit" value="Add task">
         <!-- <i class="pi pi-plus" style="font-size: 1rem"></i> -->
      </div>
   </div>
</template>

<style scoped>
   .addtask-container {
      margin-top: 20px;
      padding: 15px;
      border-style: dashed;
      border-color: #E0E0E0;
      border-width: 2px;
      border-radius: 8px;
      /* box-shadow: 0px 0px 5px 0px rgba(0,0,0,0.15); */
      display: flex;
      flex-direction: column;
   }

   .add-title p {
      font-size: 0.8rem;
      color: #686D76;
      padding-bottom: 5px;
      margin-bottom: 10px;
   }
   .addtask-text input{
      border: 1px solid #E0E0E0;
      border-radius: 5px;
      font-size: 1rem;
      padding: 10px;
      width: 100%;
      margin-bottom: 10px;
   }
   .addtask-text select{
      border: 1px solid #E0E0E0;
      border-radius: 5px;
      font-size: 1rem;
      padding: 10px;
      width: 100%;
      margin-bottom: 10px;
   }
</style>