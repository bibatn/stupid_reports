Объект Publisher в in_uvc содздается с использованием пакета image_transport:
image_transport::Publisher vpub;
Объект Subscriber в segmentation_trt создается с использованием стандартного пакета rclcpp:
rclcpp::Subscription<sensor_msgs::msg::Image>::SharedPtr sub_;
Publisher из модуля image_transport является оберткой над Publisherom из rclcpp с выставлением определенных параметров.
Авторы модулей не договаривались по вопросу какие параметры должны быть выставлены для оптимальной конфигурации.
 
