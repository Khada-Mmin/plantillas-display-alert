/*estas son plantillas para los displayalert*/

                                                      /*plantilla 1*/
<ContentPage.Resources>
    <ResourceDictionary>
        <Style x:Key="CustomDisplayAlertStyle" TargetType="Label">
            <Setter Property="BackgroundColor" Value="LightGray" />
            <Setter Property="TextColor" Value="Black" />
            <Setter Property="FontAttributes" Value="Bold" />
            <Setter Property="FontFamily" Value="Arial" />
            <Setter Property="FontSize" Value="18" />
            <Setter Property="Margin" Value="20" />
        </Style>
    </ResourceDictionary>
</ContentPage.Resources>


/*--------------------------------------------------------------------------------------------------------------------------------------------------------*/
/*como mandarla a llamar*/

async void ShowCustomDisplayAlert()
{
    await DisplayAlert("Título", "Mensaje", "Aceptar", "Cancelar", "default", new AlertArguments
    {
        Style = (Style)Resources["CustomDisplayAlertStyle"]
    });
}




/*-------------------------------------------------------------------------------------------------------------------------------------------------------*/
                                                        /*plantilla 2*/
<ContentPage.Resources>
    <ResourceDictionary>
        <Style x:Key="CustomAlertStyle" TargetType="ContentView">
            <Setter Property="BackgroundColor" Value="#FFEEEEEE" />
            <Setter Property="Padding" Value="20" />
            <Setter Property="CornerRadius" Value="10" />
            <Setter Property="HorizontalOptions" Value="Center" />
            <Setter Property="VerticalOptions" Value="Center" />
            <Setter Property="WidthRequest" Value="300" />
        </Style>
    </ResourceDictionary>
</ContentPage.Resources>
