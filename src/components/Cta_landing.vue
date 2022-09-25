<script setup>
    defineProps({
      btn_text: {
        type: String,
        required: true,
      },
    });
    </script>
    
    <template>
      <button>{{ btn_text }}</button>
    </template>
    
    <style scoped>
    button {
        background: #121212;
        color: white;
        border: 2px solid #FE6535;
        border-radius: 4px;
    }
    </style>
    