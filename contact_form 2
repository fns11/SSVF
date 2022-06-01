import streamlit as st 

st.title("SSVF Forms Selection")

#with st.form(key = "form1"):
my_form = st.form(key = "form1")
name = my_form.text_input(label = "Enter your name")
number = my_form.slider("Enter your age", min_value=10, max_value = 100 )
submit = my_form.form_submit_button(label = "Submit this form")

col1, col2 = st.beta_columns(2)

with col1:
    with st.form('Form1'):
        st.selectbox('Select your living status', ['Renting', 'Looking to Rent'], key=1)
        st.slider(label='Select intensity', min_value=0, max_value=100, key=4)
        submitted1 = st.form_submit_button('Submit 1')

with col2:
    with st.form('Form2'):
        st.selectbox('Select When you finished application', ['Complete', 'Incomplete'], key=2)
        st.slider(label='Select Intensity', min_value=0, max_value=100, key=3)
        submitted2 = st.form_submit_button('Submit 2')

st.text(number)

st.markdown("Forms Inside")

with st.form(key='columns_in_form'):
    cols = st.beta_columns(5)
    for i, col in enumerate(cols):
        col.selectbox(f'Make a Selection', ['click', 'or click'], key=i)
    submitted = st.form_submit_button('Submit')
