# Stramlit

## 使用

### 命令行

```shell
streamlit run your_script.py [-- script args]
python -m streamlit run your_script.py
streamlit run https://raw.githubusercontent.com/streamlit/demo-uber-nyc-pickups/master/streamlit_app.py
```

### write

```python
import streamlit as st

st.write("Here's our first attempt at using data to create a table:")
```

### df

```python
dataframe: Dataframe = pd.DataFrame(...)
st.dataframe(dataframe.style.highlight_max(axis=0))
st.table(dataframe)
st.line_chart(chart_data)
```

## widgets

```python
x = st.slider('x')
st.write(x, 'squared is', x * x)

st.text_input("Your name", key="name")
```

## 参考

- [Streamlit Documentation](https://docs.streamlit.io/library/get-started/create-an-app)