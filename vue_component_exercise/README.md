### Component练习
可以添加、删除、展示quote。预览点击[此处](https://htmlpreview.github.io/?https://github.com/ginnko/front-end-demos/blob/master/vue_component_exercise/index.html)。  

主要功能由以下组件完成：
- App.vue: Header、NewQuote、QuoteGride三个组件的父组件，定义了quotes、maxQuotes两个核心data；
- Header.vue: 负责显示承载条状态，父组件通过props向该组件传递quotes.length和maxQuotes两个数据；
- NewQuote.vue: 负责创建新的quote，父组件通过监听quoteAdded事件，获取新的quote并加入quotes数组中；
- Quote.vue: 负责承载和显示单个quote，使用slot从其父组件QuoteGrid中获取quote；
- QuoteGrid.vue: 负责循环quotes数组展示和删除的平台。1.通过props将quote从App组件中传递到该组件，作为slot的接收内容显示在Quote组件中；2.使用native修饰符在该组件上监听其包含的各个quote是否发生了点击（删除），利用deleteQuote事件获取被删除的quote的index，在App组件中实际删除。