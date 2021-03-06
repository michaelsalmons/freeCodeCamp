---
title: Enumerables
localeTitle: enumerable
---
## المتعدادات (التعداد)

في لغات البرمجة الشيئية ، ستستخدم "loop" لتنفيذ نفس الإجراء مرارا وتكرارا على جزء من البيانات ، في Elixir لأن المتغيرات هي غير قابلة للتغيير ، غير ممكن لإنشاء حلقة tradational ، بدلا من Elixir وغيرها من لغات البرمجة الوظيفية تعتمد على العودية. مع العودية سوف تقوم بتنفيذ نفس الإجراء فوق كل عنصر في قائمة دون الحاجة إلى تغيير متغير. مكتبة Enum التي بنيت في الإكسير يجعل هذا سهلا.

## مثال

باستخدام `Enum.map` يمكنك تشغيل وظيفة مجهولة (وظيفة ليست داخل وحدة نمطية) تمر فوق كل عنصر في قائمة. هذا ينجز نفس المهمة مثل حلقة tradational دون الحاجة إلى تحوير متغير تراكم.

 `iex> Enum.map([1, 2, 3], fn(x) -> x * 2 end) 
 [2, 4, 6] 
` 

## طرق في وحدة التعداد

تحتوي وحدة Enum على أكثر من 70 وظيفة مختلفة لاستخدامها في Enumerables ، وستدرجها جميعًا هنا ستحتاج إلى بضع صفحات. بدلاً من ذلك ، دعنا نلقي نظرة على الوظائف الأكثر استخدامًا في وحدة التعداد.

### Enum.map

يتم تشغيل `Enum.map` وظيفة مجهول أو تم التقاطها عبر قائمة.

 `iex> Enum.map([5, 10, 15, 20], fn(x) -> x * 2 end) 
 [10, 20, 30, 40] 
` 

#### معلومات اكثر:

*   [elixir-lang.org | العودية](https://elixir-lang.org/getting-started/enumerables-and-streams.html)
*   [hexdocs | التعداد](https://hexdocs.pm/elixir/Enum.html)