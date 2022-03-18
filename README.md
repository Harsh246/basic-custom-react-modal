# basic-custom-react-modal



{ create a show state and toggle it}
<br>

state={
      modal: {
               show: true,
               title: 'ye sab doglapan hai',
               description:'Bhai kya kar raha hai tu' 
             }
      }
      
<br>
 closeModal = () => {
 this.setState({
                      modal:
                      {
                            show: false,
                            title: 'ye sab doglapan hai',
                            description:'Bhai kya kar raha hai tu' 
                      }
                 });
                 
<br>
      ----------------------------------------------------------------------------------------------------------------------
      
<br>
      
{/*  conditional rendering of modal based on state. */}
      
        {show ? <Modal title={modal.title} description={modal.description} close={this.closeModal} /> : null}
        
