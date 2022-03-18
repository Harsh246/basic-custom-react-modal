# basic-custom-react-modal



{ create a show state and toggle it}

state={
      modal: {
               show: true,
               title: 'ye sab doglapan hai',
               description:'Bhai kya kar raha hai tu' 
             }
      }
      
 closeModal = () => {
 this.setState({
                      modal:
                      {
                            show: false,
                            title: 'ye sab doglapan hai',
                            description:'Bhai kya kar raha hai tu' 
                      }
                 });
      ----------------------------------------------------------------------------------------------------------------------
      
{/*  conditional rendering of modal based on state. */}
      
        {show ? <Modal title={modal.title} description={modal.description} close={this.closeModal} /> : null}
        
