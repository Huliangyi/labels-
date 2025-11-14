傅里叶变换公式如下：
$$
\mathcal{F}(\omega) = \int_{-\infty}^{\infty} f(t) e^{-i\omega t} dt
$$



# markDown-render

markdown-render katex

## 公式语法

markdown 中使用 LaTeX (KaTeX) 语法来显示复杂的数学公式。你需要在公式的两边加上两个美元符号 $$ (块级公式) 或一个美元符号 $ (行内公式) ，然后输入 LaTeX 代码。

### 行内公式

输入方式为 `$公式内容$` ，示例：$\sqrt{3x-1}+(1+x)^2$，可以在行内输入，前后有文字也可以解析。

### 块级公式

块级公式是需要 $$ 顶格写，才会进行解析，解析后，公式居中展示，示例：

$$

\begin{array}{c}

\nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} &
= \frac{4\pi}{c}\vec{\mathbf{j}}    \nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\

\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\

\nabla \cdot \vec{\mathbf{B}} & = 0

\end{array}

$$

**GitCode 会把公式解析成居中显示，而且支持公式间的换行，Gitee 不能正确渲染上面的块级公式。**

源码：

```
$$\begin{array}{c}

\nabla \times \vec{\mathbf{B}} -\, \frac1c\, \frac{\partial\vec{\mathbf{E}}}{\partial t} &
= \frac{4\pi}{c}\vec{\mathbf{j}}    \nabla \cdot \vec{\mathbf{E}} & = 4 \pi \rho \\

\nabla \times \vec{\mathbf{E}}\, +\, \frac1c\, \frac{\partial\vec{\mathbf{B}}}{\partial t} & = \vec{\mathbf{0}} \\

\nabla \cdot \vec{\mathbf{B}} & = 0

\end{array}$$
```

## 说明

异常文档链接： https://gitcode.com/openharmony/docs/edit/master/zh-cn/application-dev/ui/state-management/arkts-two-way-sync.md 

导致渲染异常的行是：

```
$$运算符为系统组件提供TS变量的引用，使得TS变量和系统组件的内部状态保持同步。

- $$绑定的变量变化时，会触发UI的同步刷新。
```

顶格写的 $$ 符号，触发了标准的 markdown 公式解析。

**处理方法：**
如果上面行中的 $$ 没有特殊用途的话，去除掉行中的 $$ 符号即可。

文档内其他的 $$ 符号，没有特殊作用的话，也可以去掉。

---

## 修复 demo 展示

# $$语法：系统组件双向同步


运算符为系统组件提供TS变量的引用，使得TS变量和系统组件的内部状态保持同步。


内部状态具体指什么取决于组件。例如，[TextInput](../../reference/apis-arkui/arkui-ts/ts-basic-components-textinput.md)组件的text参数。


> **说明：**
>
> $$还用于[@Builder装饰器的按引用传递参数](arkts-builder.md#按引用传递参数)，开发者需要注意两种用法的区别。


## 使用规则

- 当前$$支持基础类型变量，以及[\@State](arkts-state.md)、[\@Link](arkts-link.md)和[\@Prop](arkts-prop.md)装饰的变量。

- 当前$$支持的组件：

  | 组件                                                         | 支持的参数/属性 | 起始API版本 |
  | ------------------------------------------------------------ | --------------- | ----------- |
  | [Checkbox](../../reference/apis-arkui/arkui-ts/ts-basic-components-checkbox.md) | select          | 10          |
  | [CheckboxGroup](../../reference/apis-arkui/arkui-ts/ts-basic-components-checkboxgroup.md) | selectAll       | 10          |
  | [DatePicker](../../reference/apis-arkui/arkui-ts/ts-basic-components-datepicker.md) | selected        | 10          |
  | [TimePicker](../../reference/apis-arkui/arkui-ts/ts-basic-components-timepicker.md) | selected        | 10          |
  | [MenuItem](../../reference/apis-arkui/arkui-ts/ts-basic-components-menuitem.md) | selected        | 10          |
  | [Panel](../../reference/apis-arkui/arkui-ts/ts-container-panel.md)         | mode            | 10          |
  | [Radio](../../reference/apis-arkui/arkui-ts/ts-basic-components-radio.md)  | checked         | 10          |
  | [Rating](../../reference/apis-arkui/arkui-ts/ts-basic-components-rating.md) | rating          | 10          |
  | [Search](../../reference/apis-arkui/arkui-ts/ts-basic-components-search.md) | value           | 10          |
  | [SideBarContainer](../../reference/apis-arkui/arkui-ts/ts-container-sidebarcontainer.md) | showSideBar     | 10          |
  | [Slider](../../reference/apis-arkui/arkui-ts/ts-basic-components-slider.md) | value           | 10          |
  | [Stepper](../../reference/apis-arkui/arkui-ts/ts-basic-components-stepper.md) | index           | 10          |
  | [Swiper](../../reference/apis-arkui/arkui-ts/ts-container-swiper.md)       | index       | 10          |
  | [Tabs](../../reference/apis-arkui/arkui-ts/ts-container-tabs.md)           | index           | 10          |
  | [TextArea](../../reference/apis-arkui/arkui-ts/ts-basic-components-textarea.md) | text            | 10          |
  | [TextInput](../../reference/apis-arkui/arkui-ts/ts-basic-components-textinput.md) | text            | 10          |
  | [TextPicker](../../reference/apis-arkui/arkui-ts/ts-basic-components-textpicker.md) | selected、value | 10          |
  | [Toggle](../../reference/apis-arkui/arkui-ts/ts-basic-components-toggle.md) | isOn            | 10          |
  | [AlphabetIndexer](../../reference/apis-arkui/arkui-ts/ts-container-alphabet-indexer.md) | selected        | 10          |
  | [Select](../../reference/apis-arkui/arkui-ts/ts-basic-components-select.md) | selected、value | 10          |
  | [BindSheet](../../reference/apis-arkui/arkui-ts/ts-universal-attributes-sheet-transition.md#bindsheet) | isShow | 10          |
  | [BindContentCover](../../reference/apis-arkui/arkui-ts/ts-universal-attributes-modal-transition.md#bindcontentcover) | isShow | 10          |
  | [Refresh](../../reference/apis-arkui/arkui-ts/ts-container-refresh.md) | refreshing | 8 |
  | [GridItem](../../reference/apis-arkui/arkui-ts/ts-container-griditem.md) | selected | 10 |
  | [ListItem](../../reference/apis-arkui/arkui-ts/ts-container-listitem.md) | selected | 10 |

- 绑定的变量变化时，会触发UI的同步刷新。


## 使用示例

以[TextInput](../../reference/apis-arkui/arkui-ts/ts-basic-components-textinput.md)方法的text参数为例：


```ts
// xxx.ets
@Entry
@Component
struct TextInputExample {
  @State text: string = ''
  controller: TextInputController = new TextInputController()

  build() {
    Column({ space: 20 }) {
      Text(this.text)
      TextInput({ text: $$this.text, placeholder: 'input your word...', controller: this.controller })
        .placeholderColor(Color.Grey)
        .placeholderFont({ size: 14, weight: 400 })
        .caretColor(Color.Blue)
        .width(300)
    }.width('100%').height('100%').justifyContent(FlexAlign.Center)
  }
}
```

