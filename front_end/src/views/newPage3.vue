<template>  
  <el-card class="box-card scrollable-card">  
    <template #header>  
      <div class="card-header">  
        <span>Card name</span>  
        <el-button class="button" text>Operation button</el-button>  
      </div>  
    </template>  
    <div v-for="o in 4000" :key="o" class="text item">{{ 'List item ' + o }}</div>  
    <template #footer>Footer content</template>  
  </el-card>  
</template>  
    
<style>  
.card-header {  
  display: flex;  
  justify-content: space-between;  
  align-items: center;  
}  
    
.text {  
  font-size: 14px;  
}  
    
.item {  
  margin-bottom: 18px;  
}  
    
.box-card {  
  width: 480px;
  height: 480px;
}  
    
.scrollable-card {  
  overflow: auto;
}  
</style>